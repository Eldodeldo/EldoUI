# Writing an EldoUI plugin

A plugin is a separate addon that builds on EldoUI. It gets a settings page in
the EldoUI options window, a row on the **Plugins** page (title, version,
author, on/off switch), optional setup pages in the installer, a line in
`/eui diag`, and the version check. Everything goes through the global
`EldoUI`.

The same calls are what EldoUI's own modules use, so a plugin looks and behaves
like the rest of the UI.

## Rules

WoW: Forever applies the Midnight addon restrictions. A plugin follows the same
rules as EldoUI itself (the design rules are in `DESIGN.md` in the repository):

- Change how things look and where they sit. Show only data the game gives
  addons. Never compute or guess hidden combat data, and never automate
  gameplay. Test values with `issecretvalue` before doing arithmetic or
  comparisons on them.
- Anything that moves, shows or hides a protected frame goes through
  `EldoUI:RunOutOfCombat(fn)`.
- Use the design system: `EldoUI:SetPanelTemplate`, `EldoUI:SetTemplate`,
  `EldoUI:CreateText`, `EldoUI:CreateStatusBar`, `EldoUI.media.accentColor`, the
  `Core/Skin.lua` kit. Never hard-code colors, fonts or textures.
- Every option row has a `desc`. Anything that acts for the player is off by
  default.
- Never call `ReloadUI()`. Mark an option `reload = true`, or call
  `EldoUI:ShowReloadPrompt(reason)`.

## A minimal plugin

`Interface/AddOns/MyBars/MyBars.toc`:

```
## Interface: 16001
## Title: My Bars
## Notes: Two extra bars for EldoUI.
## Author: You
## Version: 1.2.0
## Dependencies: EldoUI
## X-Min-EldoUI: 0.6.0

MyBars.lua
```

`MyBars.lua`:

```lua
local E = EldoUI
if not (E and E.apiVersion and E.apiVersion >= 1) then return end

local M = E:NewModule("MyBars", {
	title = "My Bars",
	desc = "Two extra bars.",
	plugin = "MyBars",          -- your addon folder name: lists you on the Plugins page
	-- version = "1.2.0",       -- optional; the .toc's Version is used otherwise
	-- minEldoUI = "0.6.0",     -- optional; or X-Min-EldoUI in the .toc
	defaults = { enabled = true, size = 32 },
})

M.options = {
	{ type = "range", key = "size", label = "Button size", min = 20, max = 48, step = 1,
		desc = "Size of every button on both bars." },
}

function M:OnInitialize() end     -- once, after the settings are loaded (self.db)
function M:OnEnable() self:Build() end
function M:OnDisable() end
function M:OnProfileChanged() self:Build() end   -- re-apply after any change
```

Your page shows in the options sidebar under **Plugins** (set `category` in
`NewModule` to put it in another group). `M.db` is your saved settings table,
per profile, filled with `defaults`.

**Events.** Register game events with `M:RegisterEvent("EVENT", fn)` in
`OnEnable`. When the module is switched off, EldoUI drops every handler it
registered while it was on, so `OnDisable` doesn't have to list them; the
next `OnEnable` registers them again. Handlers registered in `OnInitialize`
stay while the module is off.

**Load on demand.** Plugins normally load before login. A plugin that loads
later (load on demand) is initialized and enabled inside `NewModule`, before
your `OnInitialize`/`OnEnable` exist: call them yourself right after you define
them when `M.active` is already true.

## The plugin record

`NewModule` with `plugin` registers the plugin. A plugin without a module (one
that only adds tags, datatexts or styles) lists itself:

```lua
EldoUI:RegisterPlugin("MyTags", {
	title = "My Tags",          -- default: the .toc Title (color codes stripped)
	version = "0.3",            -- default: the .toc Version
	author = "You",             -- default: the .toc Author
	desc = "Extra text tags.",  -- default: the .toc Notes
	minEldoUI = "0.6.0",        -- default: the .toc X-Min-EldoUI
	url = "https://...",        -- default: the .toc X-Website
})
```

| Call | What it does |
|---|---|
| `E:GetPlugin(addon)` | the record: `title`, `version`, `author`, `desc`, `url`, `minEldoUI`, `tooOld`, `modules` |
| `E:IteratePlugins()` | `addon, record` in registration order |
| `E:CompareVersions(a, b)` | -1, 0 or 1 (`"1.2"`, `"v1.2.3"`, `"0.6.0-beta2"` all read); nil when one isn't a version |
| `E:IsVersionAtLeast(v)` | true when this EldoUI is that version or newer (a `dev` checkout always is) |
| `E.version`, `E.apiVersion` | EldoUI's version string, and the API version (raised when a documented call changes) |

When `minEldoUI` is newer than the installed EldoUI, the player gets one chat
line at login, and the Plugins page and `/eui diag` show the warning. The
plugin is not switched off: check `E:IsVersionAtLeast` before you use a newer
call.

Your addon folder name must not start with `EldoUI_`: that prefix is reserved
for EldoUI's own module addons, which are not listed as plugins.

## Settings page

`M.options` is a list of rows; `Core/Config.lua` (top of the file) documents
every row type and field. The ones you need most:

```lua
M.options = {
	{ type = "tab", label = "Display" },                -- optional tabs
	{ type = "header", label = "Size" },                -- a section
	{ type = "toggle", key = "showText", label = "Show text", desc = "..." },
	{ type = "range", key = "size", label = "Size", min = 10, max = 40, step = 1, desc = "..." },
	{ type = "select", key = "anchor", label = "Grow", values = { up = "Up", down = "Down" }, desc = "..." },
	{ type = "color", key = "color", label = "Colour", desc = "..." },      -- { r, g, b }
	{ type = "media", key = "font", label = "Font", mediaKind = "font", desc = "..." },
	{ type = "execute", label = "Test", desc = "...", func = function() end },
	{ type = "description", label = "Free text." },
}
```

`key` is a dotted path into `M.db`. Useful fields: `desc` (required),
`dependsOn = "otherToggle"`, `hidden`, `disabled`, `requires`, `reload = true`,
`cog = { ... }` for rare settings. `M.options` may be a function that returns
the table (built the first time the page opens).

Your own page outside a module: `E:RegisterConfigPage(id, title, options,
targetFn, refreshFn, order)`; `targetFn` returns the table the keys point into,
`refreshFn` runs after every change.

Account-wide data that must not change with the profile:
`E:RegisterGlobal(namespace, defaults, { title = "...", share = true })`, read
with `E:GetGlobal(namespace)`. Per character: `E:RegisterPrivate(namespace,
defaults)` and `E:GetPrivate(namespace)`.

## Setup pages (installer)

A plugin or module can add pages to the setup. They are steps of the EldoUI
installer, between Convenience and Finish, in the same window (the
`E.WindowKit` shell). The page's Apply button is the only thing that runs its
`Apply`: Finish never applies a page on its own. A page the player looked at
and left counts as answered; pages the player never reached show after
Finish, before the reload question, in the plugin setup window. A plugin installed later gets
its pages once at the next login (the player can turn that off on the Plugins
page). Each page is asked once per character; raise `version` to ask again.

```lua
EldoUI:RegisterInstallStep({
	key = "MyBars:layout",      -- unique
	plugin = "MyBars",          -- or module = "MyBars"
	title = "Bar layout",
	short = "Bars",             -- short label (default: title)
	desc = "Pick how your extra bars sit.",
	order = 100,                -- lower first
	Build = function(frame, kit)        -- once; draw into frame
		frame.compact = kit.Check(frame, "Compact bars", "Smaller buttons, no gaps.", function(on)
			frame.choice = on
		end)
		frame.compact:SetPoint("TOPLEFT")
	end,
	Refresh = function(frame) end,      -- every time the page shows
	Apply = function()                  -- only when the player clicks Apply (out of combat)
		M.db.size = 26
		M:OnProfileChanged()
	end,
	HasChoice = function() return true end,   -- false hides Apply
	Summary = function() return "Bars: compact" end,
	when = function() return true end,        -- false leaves the page out
	version = 1,
})
```

A page without `Build` can give `text = "A paragraph."` instead. A page without
`Apply` is information only (Next). Pages never change anything on their own:
only Apply does.

`kit` has `kit.Text(parent, size, text)`, `kit.Paragraph(parent, size, text)`,
`kit.Secondary(fontString)`, `kit.Button(parent, label, width, onClick)`,
`kit.Check(parent, label, desc, onClick)` and `kit.Accent()`, all in the EldoUI
look. `E:GetInstallKit()` returns the same table.

For installer code: `E:GetPluginInstallerPages({ pending = true, plugin = addon })`
gives the pages in order (every field above filled in, plus `owner`, the
plugin's title), `E:SetInstallStepState(key, "applied" | "skipped" | "seen")`
records an answer, `E:GetInstallStepState(key)` reads it, and
`E:RunPluginSetup(onDone, { all = true, plugin = addon })` shows them in the
plugin setup window. `/eui plugins setup [name]` and the Plugins page run them
again.

A module can still define `function M:OnInstall()`; it runs at the installer's
Finish on a fresh profile.

## Other addons that do the same job

When another addon does the same job as your module, EldoUI steps back for
it, lists it on the Other addons page and in `/eui addons`, and lets the
player pick who handles the job (`Core/AddonConflicts.lua` has the details).
Declare it in one of three ways:

```lua
-- 1. The whole module stays off while one of these addons is loaded
--    (addons that own the same frames). Folder names, as in the TOC file.
local M = EldoUI:NewModule("MyBars", { title = "My Bars", conflicts = { "Bartender4", "Dominos" } })

-- 2. Only one part stands back (scope "overlap"); the rest keeps running.
EldoUI:RegisterCompetitor({
	addon = "SomeBarAddon",           -- folder name
	module = "MyBars",
	feature = "pagearrows",           -- your own key for the part
	scope = "overlap",
	label = "Page arrows",            -- what overlaps, in player words (shown)
	active = function()               -- optional: false while the other addon
		local db = _G.SomeBarAddonDB  -- has this job switched off; read its
		return not (db and db.arrows == false) -- saved settings, never write them
	end,
	exclusive = true,                 -- optional: both can't run on the same
	                                  -- frames, so picking yours turns it off
	note = "SomeBarAddon draws its own page arrows.", -- for maintainers, never shown
})

-- 3. No other addon does this (the absence is a decision), or your module
--    is made to work next to other addons and never stands back.
EldoUI:NoKnownCompetitor("MyBars", "Bars only EldoUI draws.")
EldoUI:MarkCompanion("MyBars")
```

The older `EldoUI:RegisterFeatureConflicts(feature, { "Addon" })` keeps working
and makes overlap entries on that feature key.

In your code, gate a part with `EldoUI:StandsBack(M, "pagearrows")` (true,
folder, title while it stands back) and refresh it in
`function M:OnStandBack(feature, standing)`, which EldoUI calls when the player
picks or another addon loads later. A whole module needs nothing: EldoUI does
not enable it while it stands back. `EldoUI:GetModuleConflict(M)` returns the
folder and the title of the addon that holds it; show the title, never the
folder. EldoUI never turns another addon on or off by itself, and neither may
a plugin: the player's click on the Other addons page or the setup's Finish
does it.

## Other hooks

| Need | Call | Documented in |
|---|---|---|
| Style presets (one-click looks on your page) | `E:RegisterStyles("MyBars", { { key, title, desc, settings = { ... } } })` | `Core/Styles.lua` |
| A datatext for the info bars | `E:RegisterDataText(name, { title, events, text = fn, tooltip = fn, onClick = fn })` | `Modules/InfoBar.lua` |
| A block on tooltips | `E:RegisterTooltipSection(key, { order, title, desc, default = "always", item = function(tooltip, link, itemID, add) end, unit = function(tooltip, unit, add) end })` | `Modules/Tooltip.lua` |
| A text tag (`[mytag]`) | `E:RegisterTag(name, function(unit, arg) end, "UNIT_HEALTH ...", { desc, category })` | `Core/Tags.lua` |
| A slash command (`/eui mybars ...`) | `E:AddCommand(name, usage, function(arg) end, group)` | `Core/Commands.lua` |
| A movable frame | `E:CreateMover(frame, "EldoUI_MyBars", "My Bars", { "CENTER", "UIParent", "CENTER", 0, 0 })` | `Core/Movers.lua` |
| A movable Blizzard window | `E:RegisterWindow({ key, frame, title })` | `Core/WindowMover.lua` |
| A glow with the player's glow style | `E:RegisterGlowUser(key, { title, desc, default })`, then `E:ShowUserGlow` | `Core/Glow.lua` |
| One-click profile for another addon | `E:RegisterAddonSetup(name, { title, available, import, export })` | `Core/AddonSetup.lua` |
| Pins and overlays on dungeon maps and the world map | `E:AddMapPinProvider(id, { order, pins = fn(provider, ctx), draw, clear })`, `E.DungeonMaps` | `docs/DUNGEON-MAPS.md` |
| Note packs on the world map and minimap (Map Notes) | `EldoUI:GetModule("MapNotes"):RegisterPack(id, { title, kind, maps = { [uiMapID] = { { x, y, label, quest, loot, note } } } })`, `:UnregisterPack(id)` | `Modules/MapNotes/Core.lua` |
| Your own pins under the one map switch | `E:RegisterMapPinLayer(id, { title, order, available, count, refresh })`, `E:MapPinGroupShown(id, "world" or "minimap")` | `Core/MapPins.lua` |
| Pages, search results, moments, option rows, row kinds, and data sources in My Adventure | `EldoUI.Adventure:RegisterSection(key, def)`, `EldoUI.LootGuide:RegisterSearchProvider(kind, def)`, `EldoUI.Adventure.Moments:Push(data)`, `EldoUI.Adventure:AddOptionRows(tab, rows)`, `EldoUI.Journal:RegisterSource(id, def)` | [wiki/my-adventure-api.md](wiki/my-adventure-api.md) |
| Lines in `/eui diag` | `E:RegisterDiagnostics("MyBars", function() return { "   line" } end)` | `Core/Diag.lua` |
| Sounds, fonts, textures | `E:RegisterMedia(kind, id, name, value)`, `E:PlayMedia(id)` | `Core/MediaRegistry.lua` |
| Events | `E:RegisterEvent(event, handler, owner)`; in a module `M:RegisterEvent(event, handler)` | `Core/Init.lua` |
| Translations | `E:RegisterLocale(code, strings)`, `E.L["text"]` | `Core/Locale.lua` |
| Results in the Finder search box | `E:RegisterFinderProvider(kind, fn, { label, order, dynamic, option })` | below, `Modules/Finder/Finder.lua` |

### Finder results

The Finder (`/eui go`, or the key on its options page) searches every
provider. A provider returns a list of entries:

```lua
EldoUI:RegisterFinderProvider("mybars", function(query)
	return {
		{ id = "mybars:reset", text = "Reset My Bars", sub = "My Bars", icon = 134400,
		  open = function() MyBars:Reset() end },                      -- a plain action
		{ id = "mybars:hearth", text = "Hearthstone", icon = 134414,
		  secure = { type = "item", item = "item:6948" } },            -- used by the player's click
	}
end, { label = "My Bars", order = 60 })
```

- Static providers (the default) are called once each time the box opens,
  without a query; EldoUI matches and ranks the text. With `dynamic = true`
  the function gets the query on every search and an entry may carry its
  own `score`.
- `open` runs on Enter or a click and must not call protected functions.
  Anything that casts, uses or runs goes in `secure` (the attributes of a
  `SecureActionButtonTemplate`: `type` plus `spell`, `item`, `toy` or
  `macro`): EldoUI lays a secure button over the row out of combat, and the
  player's click or Enter press is the action. Secure entries never show in
  combat; mark a plain entry `combat = false` when it must not run in combat
  either.
- `second = { label, func }` is the Shift+Enter action (a waypoint, a copy).
- Each kind gets its own on/off row on the Finder page (`option = false`
  leaves it out). Register at load or in `OnInitialize`.

## Version check

When the player has the version check on (Plugins page, on by default), EldoUI
sends one short addon message (prefix `EldoUIVer`) to the guild at login and to
the group when the player joins one:

```
1;<EldoUI version>;<plugin>=<version>,<plugin>=<version>
```

Only versions are sent, never combat data. Nothing is sent in combat, while the
client restricts addon messages (boss encounters, PvP matches, chat lockdown)
or more than once a minute per channel; a message held back goes out when the
restriction ends. Every registered plugin with a readable version is included.
When someone in the guild or group has a newer EldoUI or a newer version of one
of your plugins, the player gets one chat line per addon and session, and the
Plugins page shows the version seen. `E:GetNewerVersionSeen(addon)` returns it.

## Checklist before you publish

- `## Dependencies: EldoUI` and a `## Version` in the .toc.
- `plugin = "<your folder>"` in every `NewModule` call.
- Every option has a `desc`; no option that does nothing.
- If another addon does the same job as your module, it is declared (`conflicts` or `RegisterCompetitor`), so EldoUI steps back for it.
- `/eui diag` shows your plugin with its version; the Plugins page switch turns
  it off and on.
- Your setup pages change nothing until Apply.
