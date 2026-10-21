# My Adventure API

How a plugin adds to [My Adventure](my-adventure.md), the journal tab of the Journal window. Read the [plugin guide](../PLUGINS.md) first: the same rules apply here.

- **Show only what the game gives you.** A page, a row, or a moment says what the game reported, nothing more. Never read the combat log, never guess kills, damage, or other hidden numbers, and never store a secret value (`issecretvalue`).
- **Navigation only.** A button may open a page, the map, or set a waypoint. It never accepts, turns in, queues, invites, buys, casts, or sends anything.
- **Use the kits.** Pages are built from `E.AdventureKit` and `E.UIKit` (see the [plugin guide](../PLUGINS.md)), so they follow the style presets, the paper look, and the accent. Never hard-code a color or a font.
- **Every option row has a `desc`.**

Everything below hangs off the global `EldoUI` (EldoUI's private table, called `E` here):

```lua
local E = EldoUI
local A = E.Adventure     -- the module: sections, moments, options
local J = E.Journal       -- the journal: rows, sources, kinds, addresses
local LG = E.LootGuide    -- the Journal window: search providers
```

The journal runs while My Adventure and the Loot Guide are both on: check `A:Running()` before you act, and `J:Recording()` before you write.

## A page: `A:RegisterSection`

A section is a page in the hub's rail. Register it at file load or later; the rail picks it up at once.

```lua
A:RegisterSection("myfishing", {
	title = "Fishing",                         -- the rail label, sentence case
	icon = "Interface\\Icons\\Trade_Fishing",  -- 16 px in the rail
	desc = "Every fish you caught, by zone.",  -- the rail row's tooltip
	group = "story",                           -- "today", "story" or "atlas" (unknown: "atlas")
	order = 80,                                -- inside the group
	build = function(parent, host)             -- once, the first time it opens
		local frame = CreateFrame("Frame", nil, parent)
		-- ... build it from E.AdventureKit / E.UIKit ...
		return frame
	end,
	show = function(frame, arg) end,           -- every open; arg comes from the route
	hide = function(frame) end,                -- optional
	refresh = function(frame, changed) end,    -- while it is open: changed.adventure, changed.settings, changed.data, ...
	count = function() return 3 end,           -- the gray number in the rail
	tabCount = true,                           -- the count also adds to the tab's number
	hidden = function() return false end,      -- hide the row for now
	words = { "fishing", "fish" },             -- /eui journey <word> and /lg <word>
	search = function(text)                    -- rows for the window's search box
		return { { title = "Deviate Fish", sub = "Fishing", icon = 133888, arg = { fish = 6522 } } }
	end,
})
```

- A section without `build` has no row, so a page that isn't ready never shows. A row with `link = function(def) end` and no `build` opens something else instead of a page (the hub's Dungeons row works this way).
- `A:UnregisterSection(key)`, `A:Section(key)`, `A:Sections()` (in rail order), `A:SectionShown(key)` (it has a row now), `A:CurrentSection()`, and `A:RefreshHub()` (counts and texts again).
- **Open it**: `A:OpenSection(key[, arg])`, or `LG:Open("adventure", key)`, `LG:Open("adventure", { section = key, arg = x })`, an address (below), or any other text, which searches the Journey.
- Another module's own hub uses the same registry: `LG:RegisterHubSection(hub, key, def)`, `LG:UnregisterHubSection(hub, key)`, `LG:OpenHubSection(hub, key, arg)`, `LG:HubContent(hub)`. `A:RegisterSection(key, def)` is `LG:RegisterHubSection("adventure", key, def)`.

EldoUI's own sections are checked under all six style presets and the ten built-in layouts. Test a section of your own the same way: no Lua error, and nothing drawn outside the window.

## Search: `LG:RegisterSearchProvider`

Adds a kind of result to the Journal window's search box and Search page (My Adventure adds "Your journal" this way).

```lua
LG:RegisterSearchProvider("myfishing", {
	title = "Your fish",          -- the category chip and header
	order = 20,                   -- among the added kinds (Your journal is 10)
	search = function(words, folded, text)
		-- words: the folded words typed; return the entries that match every word, best first
		return { { name = "Deviate Fish", sub = "Caught in the Barrens", icon = 133888, fish = 6522 } }
	end,
	open = function(entry) A:OpenSection("myfishing", { fish = entry.fish }) end,
})
```

Entries need a `name`; `sub` and `icon` are optional, and any other field comes back to `open`. At most 50 are kept. Fold your own texts with `LG:Fold(text)` (`E:FoldText`) so accents and case match what was typed. `LG:UnregisterSearchProvider(kind)` removes it. The Loot Guide's own kinds (`all`, `instance`, `boss`, `quest`, `place`, `item`) can't be replaced.

## Moments: `A.Moments:Push`

A moment is a short card in the alert lane. It shows a fact the journal or your plugin just saw, and its buttons only navigate.

```lua
A.Moments:Push({
	kind = "keepsake",            -- level, zone, dungeon, goal, rested, keepsake, note (the player's ticks), reminder, brief, or your own
	title = "A rare catch",
	text = "Deviate Fish in the Barrens.",
	icon = 133888,
	seconds = 6,                  -- how long it stays (default: the player's setting)
	key = "myfishing:6522",       -- a newer moment with the same key replaces this one
	address = J:Address("section", "myfishing"),   -- what its Show button opens
	actions = { { label = "Open", func = function() A:OpenSection("myfishing") end, tip = "Opens your fish." } },
	sound = "none",               -- a media id, or "none"
	camera = false,               -- true adds the screenshot button (a click takes it, never by itself)
	always = false,               -- true shows it even while Moments is off (reminders only, please)
	now = false,                  -- true skips the combat and dungeon hold
})
```

It returns `"card"`, `"lane"`, `"notifications"`, `"waiting"`, or `"held"`, or `nil` when moments are off or the player switched that kind off. Moments wait for combat to end and are held in a dungeon until you leave, unless `now` is set. `A.Moments:Dismiss(key)` closes one. Other fields: `note`, `fanfare` (the Fanfare source that already reacts to the same game event, so the card stays quiet), `closable`.

## Option rows: `A:AddOptionRows`

Adds rows to a tab of My Adventure's settings page: `journal`, `story`, `next`, `moments`, `tracker`, `safe`, or `data`.

```lua
A:AddOptionRows("data", {
	{ type = "header", label = "Fishing" },
	{ type = "toggle", key = "myfishingMoments", label = "Moments for rare fish",
		desc = "A moment when you catch a fish you never caught before." },
})
```

Rows use the normal option row types ([plugin guide](../PLUGINS.md#settings-page)), and every row needs a `desc`. Their `key` is a dotted path into My Adventure's settings (`EldoUI.db.modules.Adventure`), so start yours with your addon's name and treat a missing value as your default. Add the rows at file load: rows added after the page was first built show after the next `/reload`. Settings that belong to your plugin alone go on your own module's page.

## Addresses: `journal:<kind>:<id>`

An address points at one thing in the journal. Links, moments, and buttons carry them, and `J:Open` opens them.

```lua
local address = J:Address("quest", 783)    -- "journal:quest:783"
J:Open(address)                            -- false when nothing can show it now
local kind, id = J:ParseAddress(address)   -- "quest", 783
J:RegisterAddress("fish", function(id, kind) A:OpenSection("myfishing", { fish = id }) return true end)
```

| Kind | Opens |
|---|---|
| `moment` | the Journey on that row (`id` is the row's `seq`) |
| `goal`, `note` | Goals or Notes on that goal or note |
| `place` | Places on that zone or dungeon |
| `fellow` | Fellowship on that companion |
| `quest` | Quests on that quest |
| `instance` | Places on that dungeon, else the Journal window's dungeon page |
| `item` | the Journal window's item page |
| `section` | that hub section, or a Catalog section (`reputation`, `crafting`, `pvp`) |

An address with no opener opens the hub on the matching section. Opening an address never does more than open a page.

To open a page by name, use `A:OpenSection(key, arg)`. `A.HubCommand(text)` is the hub's own `/eui journey` handler (it opens a section, or searches for the text); call it only for a button that does what the player would type.

## Rows and sources: `E.Journal`

The journal stores rows of kinds (`J:Kinds()` lists them). A plugin can add its own kind and feed rows through a source.

```lua
J:RegisterKind("fish", {
	group = "deeds",                  -- growth, gear, deeds, places, people, notes (the Journey filter)
	icon = 133888,
	show = "always",                  -- which detail setting shows it
	worth = 1,                        -- 3 keeps it longest when the journal is full; 1 may roll up
	rollup = true,                    -- may fold into its chapter's summary once two levels behind
	fields = { { "fish", "n" }, { "name", "i" } },   -- n number, s string, i a name kept once, b boolean
})

J:RegisterSource("myfishing", {
	title = "Fish you caught",        -- shown in "What the journal reads"
	module = "MyFishing",             -- the source is live only while this module is on
	kinds = { "fish" },
})

-- When the game tells you about a catch:
J:Emit("myfishing", { kind = "fish", id = lootGUID, fish = 6522, name = "Deviate Fish" })
```

- `J:Emit(id, row)` stores a row once: `row.id` makes the reference `"<source>:<id>"`, so the same catch is never stored twice. Place, level, and time default to where you are and now; a secret value is dropped. It does nothing while the journal does not record (`J:Recording()`) or the source's module is off.
- A source that keeps its own dated records answers `read = function(charKey, from, to, opts) return rows end` instead of emitting, and the Journey shows those rows without storing them twice. Further fields: `summarize` (numbers and names for the story, never text), `goals = { [kind] = function(charKey, target) return have, need end }`, `places`, `people`, `since`, and `scope = "account"`. The full list is at the top of `Modules/LootGuide/Adventure/Sources.lua`.
- `J:Changed(id)` tells the pages your source's data changed (one redraw later).
- Reading: `J:Rows([charKey, from, to])` (the journal's own rows), `J:Timeline([charKey, from, to, filter])` (own rows and every live source's), `J:Row(charKey, seq)`, `J:Facts([charKey])`, `J:Char([charKey])` (the saved record; treat it as read-only).
- Callbacks: `J.RegisterCallback(owner, event, fn)` with `"Logged"(charKey, row)`, `"Changed"(ids)`, `"Redraw"(what)`, `"Started"`, `"Stopped"`, and `"Cleared"(charKey)`; moments add `"Moment"(data)` and `"Keepsake"(row)`.

A plugin's rows are part of the journal's 1.5 MB budget per character. Keep rows small (ids and short names; the `i` field type keeps a name once) and let ordinary rows roll up.

## Checklist

- The page works under every style preset and layout, and every text goes through `L[]` (story text is English data).
- Nothing reads the combat log, `PARTY_KILL`, or `UNIT_DIED`. The journal itself is held to the same rule.
- No secret value is stored or used as a table key.
- Buttons only navigate. A moment with `always = true` is a reminder the player asked for.
