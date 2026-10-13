# Changelog

All notable changes to EldoUI, newest first. Each version starts with its highlights, followed by what is new, what was improved, and what was fixed. Versions are listed as `[version] - date`.

The in-game **What's New** page (`/eui whatsnew`) shows the highlights of each version.

## [Unreleased]

### Improved
- Accent colors read better as text: with a dark accent such as Crimson or Violet, titles, active tabs, links and highlighted words use a lighter shade of the same color, while bars, lines and swatches keep the color you picked.
- Status colors are easier to tell apart with color blindness: the "good" green leans toward blue-green, and the good, warning and problem inks on parchment pages are teal, olive brown and wine.
- One "Copy settings from" button on every page with several frames of one kind: Unit Frames, Group Frames (each section), Nameplates (each plate type), Action Bars, Combat Text areas, Info Bar panels, Aura Groups and Tracking Bars. Before anything is copied, it shows which settings will change and asks to confirm; the on/off switch and the position stay as they are.
- Danger Alerts has six style presets (Standard, Quiet, Loud, Raid focus, Explorer, Barnyard) that pick the sounds, the flash and which alarms are on; your spell list stays as it is.
- Party Quests is on by default, and so is Sync with group: it shares your quest progress with group members who run EldoUI, as addon messages only, never in chat. It stays silent in battlegrounds and arenas, and in raids while Hide in raids is on.
- Chat guild mutes: when Decline their group invites or Decline their duels turns someone away, one chat line names who and which muted guild (both still off by default).
- Clearer page names in the settings: Character is now Character Panel, Characters is now Alts and Alerts and Messages is now Messages. Your settings and `/eui` words stay the same, and the search still finds the old names.
- Windows: one Move Blizzard windows switch with a tick for each window under it. Ticking a window is all it takes; its Blizzard UI switch follows on its own. Your current choices carry over, and the mouse, scale, placing and fading settings moved to a Behavior tab.
- Tweaks is now part of Quality of Life: one page with Interface, Social, Quests, Travel and Sound and misc tabs. Every setting carries over; if one of the two was switched off, its features stay off. `/eui tweaks` still opens the page.
- Visibility settings: the separate instance options are now one "In instances" choice (Same as outside, Always shown, Fade, Hide or Only there). Your earlier choice carries over.
- Options window: the arrow keys and Enter move through the menu only after you click in it or in the search box. Otherwise they reach the game, so you can still move your character while the window is open.
- The Legacy Planner has the same keys as the options window: Ctrl+F puts the cursor in the Challenges search, and Esc clears the search before it closes the window. The keys only work out of combat, and every other key still reaches the game.
- XP and Reputation Bars, Raid Tools, the damage meter and the Cooldown Manager viewers now use the same Visibility settings as the rest of EldoUI (preset, Show, the extra rules behind the gear, faded opacity). Your Hide in combat, mouse-over and opacity choices carry over.
- Importing: one Import and export page with one paste box for every string (EldoUI, EllesmereUI, ElvUI and Edit Mode). It tells which kind you pasted and shows what it imports before you click Import. The separate "Import from other UIs" page is gone; its choices are on the same page.

### Fixed
- Frames faded out by their Visibility rule no longer catch clicks meant for the game world or other windows. They take the mouse again as soon as they show, and "Mouse over" frames still answer the cursor. The Info Bar's Hearthstone button follows its bar the same way.
- Map Notes City services: mount vendors and stable masters no longer show as innkeepers.

## [0.6.5001] - 2026-10-13

### Highlights
- **Dungeon Routes on your map.** Press M inside a dungeon to see its floor with your route. Edit routes with notes and drawings, and send them to your group with one click.
- **18 new modules**, including the Profession Planner, Raid Loot, Appearances, Finder, Macro Editor, Fishing, Streamer Mode, Transport Maps, and Ready Check Report.
- **Accessibility and visibility.** A High contrast art style, large text, color-blind safe colors with shape marks, sound cues, and a new Visibility page with HUD presets such as Quiet and OLED.
- **A calmer, consistent config window** with keyboard navigation, a Recent changes list with Undo, and one shared look for every button, dialog, and window.
- **The Loot Guide speaks nine more languages** on German, French, Spanish, Brazilian Portuguese, Russian, Korean, and Chinese game clients.

### New
- **Profession Planner** (`/eui plan`): pin recipes with a number of crafts and see every reagent, including sub-reagents, with what you have in your bags, bank, and on your other characters. Includes recipe cooldowns, missing prices, a tracker, a reagent tooltip line, "Send to Shopping" for an auction house shopping list, and a leveling plan with the cheapest recipes to a target skill.
- **Fishing** (off by default, `/eui fish`): fishing mode turns one key into Cast Fishing, and into "loot the bobber" while it is out. Adds a fishing bar with Cast, Lure, and Swap, an optional louder splash, double right-click casting, and a catch log per zone and spot with catches per hour and skill-ups. Set the key by pressing it. One action per press; nothing casts by itself.
- **Raid Loot**: import softres.it and That's My BiS exports to see "SR:" and "TMB:" lines on item tooltips and beside each loot roll. The Loot Guide marks items you reserved, and a GDKP ledger tracks sales, the pot, cuts, and payouts with a text export. Posting to the group is one click and off by default. EldoUI never rolls for you.
- **Appearances**: a small mark on item buttons in bags, vendors, loot, rolls, mail, and the auction house shows whether you have the item's look, have it from another item, or can't collect it. Adds an "Appearance:" tooltip line and a looks count per set in the Loot Guide.
- **Finder** (`/eui go` or a key of your choice): one search box for game panels, EldoUI settings, mounts, toys, bag items, macros, places, commands, and quick sums. Using anything is always your own click or Enter, out of combat.
- **Macro Editor** (`/eui macros`): a wider editor next to Blizzard's macro window with a live syntax check, a condition builder, an icon search by spell or item name, Duplicate, and five looks. Saving happens out of combat.
- **Streamer Mode** (`/eui streamer`): party members show as aliases on EldoUI frames, tags, tooltips, and chat. Optional generic names for everyone else and hidden names above heads, restored when you turn it off.
- **Chat Input**: messages longer than the chat limit are sent in parts, one per Enter, on the same channel. Adds a letter counter, undo and redo (Ctrl+Z, Ctrl+Y), draft recovery (Ctrl+Shift+Z), and an optional "is typing" line for party members who also use EldoUI.
- **Zone Quests** (`/eui zones`): a Zones section in the Loot Guide Catalog with every zone's done and remaining quests and their givers, optional quest giver pins on the world map, and a "Quests done / total" line in the zone tooltip.
- **Quest Starter Drops**: creatures that can drop a quest-starting item say so in their tooltip and with a small icon on their EldoUI nameplate.
- **Party Quests** (off by default): in a group, compare your quests with your party (Shared, Only mine, Only theirs), with one-click Share and Ask, opt-in progress sync, progress popups, and a group summary.
- **NPC Dialog** (off by default): a large, readable dialog view for quest and gossip NPCs with numbered choices, Space to continue, and Esc to leave. It never accepts, completes, or picks anything for you.
- **Transport Maps**: flight masters, boats, zeppelins, the Deeprun Tram, and portals on the world map, with destinations, learned flight times, waypoints, and a Routes tab.
- **Ready Check Report**: on a ready check, one panel lists each member's missing buffs, flask or elixir, Well Fed, and shared durability, with one-click "Post to group". Sharing your own durability and version is a "Share mine" button; nothing is sent when a ready check starts.
- **Cast Tooltips and Mob Abilities**: hover the target or focus cast bar for the spell's tooltip. NPC tooltips list the abilities you saw that mob cast, and reputation turn-in items show where they go and the standing they give.
- **Spell Efficiency**: spell tooltips show damage or healing per second and per mana, and the mana cost as a share of your pool.
- **Hardcore**: a death log and death alert cards for announced Hardcore deaths, a one-click "Tell the guild" card after your own death, PvP flag warnings, and Self-Found reminders.
- **Split Timer**: a leveling timer that races your best, a card at each level-up, and a Splits tab in the Characters window.
- **Dungeon Routes**:
  - Press M inside a dungeon to see its floor with your route and position. "Game map" takes you back to Blizzard's map.
  - Edit routes with notes, arrows, and free-hand lines, with undo. Drag pulls to reorder them, and move, join, or delete them from the pull menu.
  - Send a route to your group with one click. Receiving is off by default, and received routes wait in "From your group" until you keep them.
  - An optional route card (off by default) shows the next pulls with Done and Back buttons.
- **Visibility page** with five HUD presets (Always, Quiet, Combat, Minimal, OLED) and one tick per module. Quiet HUD fades EldoUI frames while you are idle, and a "Show the HUD (hold)" key brings them back, also in combat. OLED care (off by default) dims the HUD when idle and shifts it by a tiny amount.
- **Accessibility**: a High contrast art style, large text up to 160 %, color-blind safe colors with shape marks (dispel colors show their dispel-type symbol, and the threat border shows "!" when you are in danger), and sound cues. The setup has a new optional Accessibility step; nothing is ticked for you.
- **Camp Helper**: an optional camp finder (off by default). Ask your guild or group for a camp, or share yours with one click; other EldoUI users get a toast with a waypoint. Nothing is sent or answered without a click.
- **Characters**: a new Crafters tab lists guild members who know a recipe, from recipe lists they choose to share. Sharing is off by default, and requests are shown, never answered automatically. Adds a "Guild crafters" tooltip line and a line in the Loot Guide's Crafting detail.
- **Tweaks**: a game settings browser (`/eui cvars`) to search, set, and restore the game's settings, including hidden combat text, chat, and camera settings. Every change can be put back, and protected settings are left out.
- **Chat**:
  - Mute whole guilds (`/eui chatguild`): their chat lines, emotes, and speech bubbles are hidden from your screen, with a log of what was hidden in the last 15 minutes. Add a guild from a player's right-click menu. Declining their invites and duels is optional and off by default.
  - Sticky channels: one tick per chat type keeps the edit box on the chat type you last used.
  - Alt-click a player's name to send them a group invite (off by default, never in combat).
  - `/eui tt` and a new key binding open the chat box to whisper your target.
  - A new "Hide other players' crafting" filter (on by default) keeps other players' craft lines out of the Loot tab. Your own crafts always show.
- **Sound and Fun**:
  - Nine new triggers: a group member levels up, a profession skill rises, a reputation standing rises, a new spell, a new flight path, a friend comes online, a wishlist item drops, a raid warning, and loss of control.
  - The friend trigger can watch guild members, friends, or both.
  - A "Take a screenshot" action per trigger, off by default.
- **Map Notes**: a new "City services" pack with trainers, weapon masters, bankers, the auction house, flight masters, and innkeepers.
- **World map**: "Show unexplored areas" shows the parts of a zone your other characters explored, dimmed.
- **Move mode**:
  - "Show test frames" shows sample unit, party, and raid frames, loot rolls, alerts, and timer bars at once.
  - The selected frame is outlined in your accent color, and frames light up when you point at them.
  - Frames attached to another frame keep up when that frame changes size, and "Match size" gives a frame another frame's width.
- **BigWigs**: a new EldoUI bar style, timing for your role, an "EldoUI - <layout>" profile, and "Restore my previous BigWigs profile" and "Re-apply to BigWigs" buttons. The installer can set BigWigs up without a saved profile string and explains its per-spec profiles.
- **Config window**: a Recent changes list with Undo for each change or all of them, and keyboard navigation (Ctrl+F to search, arrow keys and Enter to move through the tree and results, Esc to step back).
- **Bags and Merchant**: items your quests or recipes still need get a lock mark, are never sold as junk, and show "Needed" in the tooltip. Gray and white items show "Safe to sell". The lock mark also shows on Blizzard's own bag slots.
- **Bags**: an optional "Move these" button (off by default) moves the items you searched for to the open trade, mail, bank, or vendor in one click, and a category header's right-click menu can move that category's items. Protected items are never moved.
- **Delete dialog**: deleting a quest item shows which quest it belongs to and whether you are on it.
- **Auction House**: tooltip prices show how old they are, and prices older than 14 days are dimmed.
- **Merchant**: an optional "Buy back this visit" button buys back what you sold at this vendor.
- **Tooltips**: alt and bank counts, auction prices, alt recipes, alt quests, and click casting bindings are now tooltip sections you can arrange in the Tooltip options. They still show when the Tooltip module is off.
- **Text tags**: new XP tags `[xp:percent]`, `[xp:remaining]`, and `[xp:rested]` for the player frame.
- **Quests**: quest giver lists show quest levels in difficulty colors, color-blind mode adds a difficulty word, and right-clicking a quest offers "Wowhead link" and "Remind me when done".
- **Friends**: a "Recently grouped" tab with Add friend, and friend notes you can edit right in the list.
- **Lua errors setting** (General > Lua errors): the game's own Lua error window is hidden by default, so no error waits for a click. EldoUI still logs every error in `/eui errors`. Show and Don't touch are the other choices.
- **Loot Guide**: the interface is now translated into German, French, Spanish (Spain and Mexico), Brazilian Portuguese, Russian, Korean, and Simplified and Traditional Chinese. Search finds items by names the client learns later, item names switch to your language without a reload, and an empty Reputation list offers "Show all factions".
- **For plugin authors**: `EldoUI:RegisterUnitEvent` and `UnregisterUnitEvent` for unit events with the game's unit filter.

### Improved
- **One look everywhere.** Every EldoUI window now shares the same buttons, inputs, checks, sliders, menus, scroll bars, and icons, and the same window and dialog shell. Questions ask in one dialog, with a clear danger button for deletes and resets.
- **Calmer options window**: white section titles, a larger page title, a sidebar grouped into Look and Setup, a default value in every tooltip, units on every slider ("85 %", "0.5 s"), rare settings folded under "More settings", tabs that explain when they have nothing to show, and a search that understands British spellings and common synonyms.
- **Themes reach every window.** The art style, accent color, and color-blind palette now apply to every window, and theme changes repaint everything at once without a reload. Dungeon maps, the chat panel, tooltips, Sound and Fun text, and the threat meter, Counters, Farming, Camp, and Raid Tools strips follow the art style.
- **Pixel-exact windows** at every resolution and UI scale; borders stay one screen pixel.
- **Style presets**: 5 to 7 presets per module, and each one sets the same switches every time.
- **Colors**: unit frames and nameplates use the Reaction colors from General > Colors (nameplates can keep their own), and text tags, the Loot Guide guild list, My Adventure, and reputation cards follow your custom class, reaction, and power colors.
- **Cooldown numbers** have one look under General > Fonts and Text, shared by action bars, aura icons, and weapon enchants. Module sizes scale with the general size, and the action bars can keep their own.
- **Money and times** read the same in the Auction House, Merchant, Trade, Bags, and the info bar.
- **Training**: the Training window docks beside class trainers, so they show one list.
- **Windows**: the `/way` paste window and the Map Notes editor are full EldoUI windows with the theme font, scroll bar, and Escape to close. Long lists scroll smoothly with the mouse wheel.
- **Smoother play**: settings changed in combat queue one refresh per module, repeated refreshes after combat run once, action bars re-apply only what changed, and the Consumable Bar, Reminders, and flight bar do less work in the background.
- **Clear options**: every option that acts for you is marked "Off by default", and buttons that wipe saved data ask before they clear anything. Settings that need another switch are grayed out with a hint saying which one.
- **Setup**: the installer's progress line animates, and What's New opens once per new version at login. The EldoUI page in the game's Settings uses the EldoUI look.
- **Small touches**: "Click Casting" is spelled the same everywhere, the quest tracker's difficulty word never wraps a title, the danger flash follows the Animations switch, and the low mana note uses your mana color.

### Fixed
- No more "seterrorhandler is forbidden for hooking" message at login.
- Class power and nameplate text no longer error when the game hides a value.
- The aura pop-in effect no longer errors on nameplates; where the game does not allow it, the effect turns itself off.
- Chat: the edit box no longer stays on screen as a dim bar over the tabs, where it could cover the Errors, Find, and Copy buttons. The General and Combat Log tabs sit at the same height as the others.
- Talent Planner: the Trees tab shows your three talent trees again.
- The AFK screen shows the full EldoUI logo instead of a squashed square.
- The world map, spellbook and talents, friends, and group finder windows can be dragged again. The Recommended setup now allows Move and scale for every Blizzard window.
- Enemy Spotter no longer shows "bad argument to min" errors.
- Friends: Blizzard's sub-tab no longer looks selected under Recently grouped.
- Auction House: the shopping list redraws when the Profession Planner fills it.
- Blizzard UI page: each section shows its current state next to its title again.
- Import: "Copy my Edit Mode layout" no longer errors when the preset layouts are not available.
- The Tooltip panel opacity now survives an art style change.

## [0.6.5000] - 2026-10-13

### Highlights
- **My Adventure**: a journal of your own journey that writes itself as you play and tells it back as a story from level 1 to 60.
- **Nameplates and frames come alive** with effects presets, 3D portraits, and the new Perl style for unit and party frames.
- **Encounter Timeline**: your boss mod's timers as icons sliding towards now.
- **Rare Scanner**, **Attunements**, **Map Notes**, **Characters**, **Combat Text**, and many more new modules.
- **A new setup wizard and options window**: step-by-step setup, a searchable sidebar tree, profiles per character and talent group, and imports from EllesmereUI, ElvUI, and Edit Mode.

### New
- **My Adventure**: a journal of your own journey as the first tab of the Journal window. It records levels, places, dungeons, quests, companions, and keepsakes from what the game shows you, and tells them as a story with chapters per level, a storybook, a Today page, a Journey page with a level river, and Next trips that suggest where to go at your level. Goals, notes, an on-screen tracker, moment cards, attunement progress, and a prep list before a dungeon are part of it. Built on Forever Journal by Ugge Zen (MIT).
- **My Adventure** also brings an import from Forever Journal (with Undo), backups with restore, exports as Markdown, a printable page, plain text, or a journal code, key bindings, an addon compartment entry, a Journal button in the game menu, a minimap button, journal lines in tooltips and Zone Info, notes on the world map, keyboard navigation, a "Where you left off" card, and a Paper page look.
- **Rare Scanner**: when a rare shows up on the minimap, a nameplate, your target, under the mouse, as your group's target, or in a yell, you get a card you click to target it and one sound. Includes an optional chat line, a tooltip line, a "Rares" data text, and an optional targeting key. Nothing is targeted, marked, or sent unless you click.
- **Encounter Timeline**: EldoUI's own timeline bar, fed by the timers DBM and BigWigs publish. Icons slide towards a now-marker with warn and bad colors, lanes, a waiting stack, and a big icon with a cooldown swipe for the next timer. Includes pull, break, and ready check rows, an optional countdown sound, test fights, six styles, and a mover in all 17 layouts.
- **Raid Tools**: `/eui pull [seconds|cancel]` starts or cancels the group pull countdown, and says why when you can't.
- **Nameplates**:
  - An Effects tab with the presets Off, Subtle, Standard, and Vivid: cast bar fade and spark, quest icon pop, aura pop-in, a threat border that can pulse at danger, "Another tank has it" for tanks, the absorb shield, the important cast glow, and the interrupter's name. The execute shade and an important cast sound are opt-in. Inspired by Plater.
  - Target highlights, "Others step back", focus as target, "Target plate details" for layouts without a target frame, sizes in combat, minor unit and pet scales, miniboss and health gradient colors, a channel color, enemy defensives, and "Fade units out of combat".
  - Blizzard's real plate size, click-through friendly plates, and Situations with separate settings for the open world, dungeons, raids, and battlegrounds. Blizzard's escort and capture bars stay visible on EldoUI plates.
  - Style filter rules gain "Is casting", "Cast is important", and "In execute range" triggers and new actions. Every layout names the nameplate style that fits it.
- **Attunements** in the Loot Guide: raid attunements, keys, dungeon chains, and class quests as a flowchart or step list with the giver, the place, and your progress. Includes an overview of your characters, a guild view, step toasts, a next-step map pin, tooltip lines, and an Attunements grid in Characters.
- **Unit Frames and Party and Raid**:
  - An Effects tab with the presets Off, Subtle, Standard, and Vivid: threat border, low health and power warnings, out-of-range fade, dead and offline looks, target change flash, fade in, aura pop-in, expiring auras, resurrection and summon pulses, and the important cast glow.
  - 3D portraits on every unit frame and on party frames, with framing, distance, rotation, and height settings.
  - A "Perl" style with a 3D portrait in its own box, a name bar with race and class, a thick health bar, and level and class badges. Look inspired by X-Perl and Z-Perl.
  - The info panel can sit over the bars as a name bar, and ready check results fade out after a time you set.
- **Map Notes**: one button on the world map shows or hides every EldoUI pin (your notes, rares, waypoints, gathering nodes, instance entrances, and HandyNotes when installed), with one tick per group, a key binding, and `/eui mapnote`. Add your own notes with Alt+right-click.
- **Deadly Boss Mods**: an EldoUI DBM profile per layout with placed timers and warnings, the EldoUI look, and quiet chat.
- **Characters**: an Alts window with an overview, search, professions, mail and auctions, quests, grids, a character page, a level log, an agenda, a guild bank view, and an opt-in guild exchange.
- **Tracking Bars**: one bar per spell for an aura's time left, stacks, cooldown, or charges, under the Cooldown Manager.
- **Cooldown Manager**: your own cooldown groups with drag and drop in move mode, free icons, per-icon looks with up to three labels, a visibility rule per group, and a layout per talent group.
- **Cooldown Pulse**: a center pulse when your own spell or item is ready, with an optional sound, spoken name, and glow.
- **Battleground Timers**: queue, entry, start, base capture, expected winner, time left, and flag timers, with a skin, move, or hide switch for Blizzard's start countdown.
- **Combat Text**: scroll areas, notifications, loot lines, warnings, nameplate numbers, an event editor, and six styles, with a hand-off from Blizzard's combat text.
- **Instances**: the hourly instance count across your characters, a run log with stats, reset notices, a Raid Tools reset button, and a battleground log.
- **Cast Bar Effects**: themed cast bars with spark, trail, shine, particles, and finish, interrupt, and pushback effects.
- **Talent Planner**: plan your talents with trees, a level guide, and saved plans, see the plan on Blizzard's talent page, and learn the next point with one click.
- **Blizzard UI page**: one switch per part of Blizzard's UI. Off leaves Blizzard's version alone; on lets you pick skin, move, hide, or replace.
- **Options window**: previews, "Copy from", a mark on changed rows (right-click resets), a resizable window, a reload banner, and a search that also finds descriptions and choices.
- **Profiles**: account and character profiles, rename, copy parts of a profile, per-character module states, profiles per talent group and content, and a class default profile for new characters.
- **Share strings**: a readable Lua export, an import checklist, and sending settings to a player, party, raid, or guild. The import window also reads EllesmereUI, ElvUI, and Edit Mode strings.
- **Setup wizard**: a step-by-step installer with per-addon setup, a BigWigs profile import, an ultrawide safe area, a Game settings step (only what you tick changes), a Chat step that can reset the chat windows first, and a Welcome step that offers the shared EldoUI profile on an alt.
- **Shared engines** with their own pages: visibility rules, glows, text tags, aura filters, media colors, number format, game fonts, and shadows.
- **Edit Mode**: EldoUI's frames inside Blizzard's Edit Mode.
- **Action Bars**: eight bars plus pet, stance, vehicle, extra ability, totem, and gamepad bars, per-bar Blizzard handling, fade and visibility rules, proc glow, Masque support, cooldown numbers, and spell rank upgrades.
- **Unit Frames**: Blizzard element switches, focus, pet, and party extras, heal prediction, text tags, element tabs, cast bar upgrades, and a fader.
- **Player Power**: a class resource bar, combo points, druid mana, the five-second rule, a GCD bar, color ranges, and extra bars.
- **Buffs and Debuffs**: EldoUI frames with right-click cancel, weapon enchants, filters, "yours first", blinking, and time bars.
- **Party and Raid**: main tanks, group pets, raid sizes, indicators, per-section layouts, and click casting bindings. **Raid Tools** adds a bar with ready check, role check, pull countdown, and markers.
- **Combat HUD**: Blizzard's damage meter, swing timer, loss of control, mirror and quest timers, and death recap skinned and placed, plus EldoUI's threat meter, combat timer, cursor ring, and crosshair.
- **Cooldown Manager**: skin and placement for Blizzard's Cooldown Manager, plus EldoUI rows for trinkets and mobility spells.
- **Aura Groups**: your own rows of aura icons, each on its own mover.
- **Quickdraw**: hold a key for a ring, fan, or grid of your own spells, items, macros, mounts, and markers.
- **Interface**: a rebuilt minimap, a second info bar, custom datatext panels, a LibDataBroker bridge, XP, reputation, honor, and pet experience bars on one mover, a movable micro menu and bag bar, the Quest Tracker, and the Maps module.
- **Chat**: saved history, search, keyword alerts with their own sounds, a spam filter, content filters, per-channel colors and mutes, link tooltips, item and spell icons, emoji, and a right panel. Chat bubbles get the EldoUI look, and Instant Messages gets group windows, contact info, and a history browser.
- **Alerts and Messages**: an alert lane, talking head, raid warnings, error and zone text, ready checks, queue popups, cutscene handling, and pings. Battle.net toasts and the GM ticket box can get their own mover.
- **Window skins** for the character window, guild, friends, calendar, group finder, PvP, bags, bank, mail, merchant, trade, auction house, NPC dialogs, and system windows.
- **Items**: bag categories, a bag bar, currencies, a guild bank cache, item cooldowns, a tint for items you already know, a merchant restock list, mail multi-select and a sent log, auction house disenchant values, full scans and crafting prices, and a Trade module with a gold trade log.
- **Loot Guide**: a loot journal, best-in-slot sets, a wishlist, search, item pages, and loot lines in item tooltips, with the separate EldoUI_LootData folder.
- **Training**: what your class trainer can teach you now and later, with costs and an ignore list.
- **Sound and Fun** (off by default): sounds, big text, and screen flashes for moments in the game, with a media library.
- **More**: an AFK screen (off by default), Pet Care for hunters, gear set buttons, Reminders upgrades, a flight timer, placement for Details!, RestedXP, BigWigs, and Questie, the "WoW Forever" art style with a bronze frame line, a Plugins page with setup pages and a version check, and language pack selection.
- **Releases**: every version is available as a ready-to-unzip `EldoUI-x.y.z.zip` on the releases page.

### Improved
- The 15 community-inspired layouts now sit on EldoUI's own placement grid, and each credits the preset that inspired it.
- EldoUI's text is in US English everywhere, like the WoW: Forever client. Settings, profiles, and saved data keep working.
- **UI scale**: EldoUI is made for 1440p, and Auto now draws that canvas on every screen, so a layout looks the same on 1080p, 1440p, and 4K. Pixel perfect for your own screen is its own choice in General > Scale, in the installer, and with `/eui scale pixel`.
- **Options window**: the sidebar is a tree that unfolds into tabs, remembers what you opened, and dims switched-off modules. Drag the corner to resize the window. Clicks land exactly where controls are drawn, and every button, tab, and menu shares one hover and pressed look.
- **One consistent look**: one button height per row, the same text grays, title sizes, and control heights everywhere, new Panel opacity and Text shadow settings, and borders that stay one screen pixel sharp in scaled windows.
- **Clearer texts**: plain-language switch descriptions on the Blizzard UI page, module names instead of code names, and group names such as "Chat and Social", "Items and Economy", and "Fonts and Text". Confirmations stay in the window instead of the chat.
- **Installer**: every layout card shows a small map of the layout, a progress line in the footer, and a "Blizzard's own UI" choice. Nothing changes until you click Apply or Finish. It opens on the first login and on every new profile until you finish or skip it.
- **Roles**: the damage, healer, and tank positions are now part of the layout, so a frame you dragged yourself stays put and Reset puts it back at its role position.
- **Fresh profiles** get the layout's sizes and module settings even when the setup is skipped, and a frame the layout hides stays hidden when you turn its module on later.
- **Layouts**: all layout presets follow the same placement rules, and styles no longer move frames.
- **The EldoUI config** opens only with `/eui`, so a stray right-click on a frame never opens it.
- **Reloads** always go through a Reload button, because WoW: Forever blocks addon reloads.
- **Profiles** save only what you changed, and switching profiles turns modules on or off without a reload.
- **Party and Raid**: the "Compact DPS" style is merged into "Minimal". The threat border and important spell glow moved to the Effects tab, and the tapped and offline colors moved to General > Colors. Saved choices move with them.
- **Nameplates**: settings the game keeps protected (max distance, plate sizes, opacity behind walls) moved to Blizzard's Options > Nameplates, and the Game settings tab points there.
- **Gear sets** equip only on your click; they never swap on their own when you change spec or stance.
- **Fair play**: the trainer's "train all" button and the styles that acted for you (fast questing, quiet mode) are gone.

### Fixed
- Borders stay one pixel thin after the UI scale changes.
- The waypoint coordinates no longer overlap raid warnings in the Eldo-Modern layout.
- A frame anchored to a missing frame falls back to its default position.
- The main chat window goes back into EldoUI's chat panel after Edit Mode changes.
- A layout preset or undo that changes the accent repaints every window at once.
- EldoUI's reset popups no longer take the popup slots the game needs for its own dialogs.
- Whisper windows have the skinned close button, and Escape closes the whisper history.
- Map widget text gets its original font back when the skin is turned off.
- "Smooth bars" on unit and group frames follows General > Textures by default.
- Blizzard's action bars, player frame, and cast bar no longer show next to EldoUI's.
- The first `/eui` after login opens the config window reliably.
- Waypoint and gathering pins in the corners of EldoUI's square minimap are no longer pulled in or hidden.
- Bag search no longer drops digits from what you type.
- Blizzard frames EldoUI moves or hides now stay put through login, `/reload`, loading screens, Edit Mode, spec changes, vehicles, pet battles, and combat.
- Moving Blizzard's party or raid frames during combat now happens when combat ends instead of being dropped.
- Many smaller fixes and polish.

## [0.5.0] - 2026-10-11

The first public version of EldoUI for WoW: Forever.

### Highlights
- A complete, modular UI with frames, bars, nameplates, chat, bags, and dozens of interface modules.
- Layout presets with one-click apply and a first-login installer.
- Move every frame with `/eui move` and share your setup as a string.

### New
- **Core**: saved settings and profiles, the module and plugin API, the EldoUI config window, movers with grid snap and nudge (`/eui move`), keybind mode (`/eui kb`) with keybind presets, share strings, the error log, `/eui` commands with an in-game help window, and a pixel-perfect 1440p scale.
- **Layouts**: layout presets with one-click apply, a first-login installer, and one-click setup for Details! and the Cooldown Manager.
- **Looks**: style presets per category, art styles, and the EldoUI media pack (fonts, bar textures, logo, and icon).
- **Frames**: Unit Frames, Party and Raid, Click-Cast Tips, Nameplates, and Action Bars.
- **Interface**: Info Bar, Minimap, Tooltip, Character window, Reminders, and Counters.
- **Social**: Chat, Instant Messages, and Friends and Social.
- **Items and economy**: Bags and bank with your other characters' items, Upgrades, Auction House, Merchant, Mail, Loot, and Mob and Loot Info.
- **Quality of life and combat**: Tweaks, Quality of Life, Enemy Spotter, and Danger Alerts.
- The EldoUI logo and an entry in the game's addon compartment.

### Improved
- Auto repair and selling gray items are on by default, with clear junk rules.
- Enemy Spotter starts at the top left, clear of the party frames.
- Loot rolls stay fully manual: automatic greed on green items is gone.

### Fixed
- Style presets and the Tooltip load again.
- Secret cast flags no longer break the cast check, and the chat error log can be closed.
- Fixes for keybind mode, instant message themes, the installer, roll arrows, the tooltip fallback, and options that did nothing.
- Character keys ignore the Forever surname, and the weapon enchant check uses the current item API.

[Unreleased]: https://github.com/Eldodeldo/EldoUI/compare/v0.5.0...HEAD
[0.5.0]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.5.0
