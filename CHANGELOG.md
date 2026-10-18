# Changelog

All notable changes to EldoUI, newest first. Each version starts with its highlights, followed by what is new, what was improved, and what was fixed. Versions are listed as `[version] - date`.

The in-game **What's New** page (`/eui whatsnew`) shows the highlights of each version.

## [Unreleased]

### New
- The keybind setup can put your known class spells on the empty buttons of their category when you apply, so every character finds them under the same keys. Buttons with your own actions keep them, nothing moves by itself later, and Take back removes the placed spells again.
- `/eui blessings` opens or closes the Blessing Plan.
- New profiles gather addon minimap buttons behind one button; the drawer opens toward the middle of the screen and closes with a click elsewhere or Escape. "Manage buttons" keeps any button on the map.
- An unfinished setup now reminds you once per login: a chat line with /eui install and a small "Finish your EldoUI setup" alert with Start or Continue setup, Later and Don't remind me. A setup you close no longer opens by itself at the next login.
- Vanilla unit-frame graphics crown the target and focus portrait of an elite with gold and a rare with silver.
- Native skins draw a thin ring around aura icons and cooldown icons; small icons keep their clean edge.
- Layout and style > UI amount: choose Essential, Moderate or Full. Each level only switches EldoUI's optional helpers on or off, shows what it changes before you apply it, marks the level recommended for your layout, and can be undone. Your frames, skin, key bindings and other addons stay as they are.
- Layout and style > Overview: your whole look on one page, with three complete looks (Structured, Focus and Portrait Forge), the layout, the UI amount and Blizzard's windows, a summary of what changes and one Apply button.
- Move mode shows your setup (EldoUI version, layout, skin, role and UI amount) at the bottom of its panel, ready for a screenshot, and "Copy setup" gives the full summary for a bug report. The Split Timer now has its box in move mode's Combat view.
- Right-click a box in move mode to pick a Layout (Horizontal, Vertical or Grid) for the Micro Menu, the Bag Bar and the action bars; the Micro Menu can also go back to Blizzard's own placement, and Options… opens its settings.

### Improved
- The second info bar now sits in the top edge of the chat window by default, so the two-bar info bar styles work in every layout. Pick "Its own mover" to place it freely; a bar you already use keeps its spot.
- The keybind setup now names Ghost Wolf, Aspect of the Cheetah and Resurrection for their categories.
- My Adventure's Parchment look prints its text as clean ink, without the dark outline that made letters run together, and a light paper wash calms the parchment grain under long text.
- On the Blizzard UI page, each Blizzard window says where its look comes from: the Blizzard windows choice, your own pick, or no EldoUI skin yet. The windows summary on the Appearance page no longer counts a window EldoUI has no skin for as skinned.
- Closing the Auction House, a vendor or your bags does less work at once, which removes a short hitch.
- The stopwatch is a compact timer in the EldoUI look: digits and buttons on one row, boxed start, pause and reset buttons with tooltips, and a slim title bar that fades in when you point at it.
- The addon button bin leaves hidden buttons hidden without gaps, finds more addon buttons, and steps aside while MinimapButtonButton or HidingBar is loaded. The "Button rail" style no longer changes how addon buttons are gathered.
- The RestedXP guide mover now covers the whole guide, including its current step card above or below it, and follows RestedXP's changes. Before your setup is done, the guide waits under the game's player frame instead of covering it. The RestedXP settings and the setup's Other addons step say which addons EldoUI places.
- Party frames with portraits now show the unit-frame graphics' portrait ring or frame, drawn inside the portrait so dense groups keep their room.
- Every skin now decides on its own how the bronze marks of the Loot Guide, NPC dialog and Party Quests and the selected tabs look; the warm skins show them in their own color.
- With the minimap buttons skin on, the addon compartment's count uses the EldoUI font.
- Section names in the options sidebar wrap to a second line with Large text instead of being cut, and a Setup reminders option on General brings the setup reminder back after "Don't remind me".
- The Shaman Totems bar has its own place in every layout, and kept totem timers sit above it.
- The Minimal unit-frame style now keeps a slim power bar, so your mana, rage or energy is always in view.

### Fixed
- The Shopping List no longer leaves an empty header on screen when nothing is pinned, also after placing frames. Right-clicking its header offers Hide again, like other EldoUI boxes.
- The mailbox toolbar now has its own row under the Inbox and Send Mail tabs instead of sharing their strip. Send Mail shows only the Sent log button on the toolbar, and the extra Sent log button over the postage is gone.
- The Talent Planner button and build bar on the game's talent window now draw above the window's own controls.
- A wide first letter of a chapter in the Book no longer runs into the words beside it.
- Player names written in Cyrillic, Korean or Chinese show their letters on nameplates instead of empty boxes, while Latin names keep the picked font.
- The Bag Bar and Micro Menu boxes in move mode now match the bars you see, so dragging and snapping line up with the buttons.
- In Blizzard's Edit Mode, the empty Bags and Micro Menu boxes no longer sit where the bars used to be while EldoUI places them; drag EldoUI's own box instead.
- A new character's intro scene no longer pauses the EldoUI setup. The setup waits until the scene and its skip question are over, and until the Escape key is released, then opens once.
- A name shown above a unit frame and the level text above its corner no longer sit under the graphics' border.
- Buffs, group pets, tanks and the second resource bar move aside when a larger minimap, a wider raid or a separate resource bar would cover them, and the healer layouts give every optional frame a spot of its own.
- Alert cards with a long text, such as "New in this version", now grow to fit their text and buttons at every text size, so they no longer run into their buttons or the card below.
- Health bars on unit frames with the Vanilla or Portrait Bars graphics no longer turn into a dark bar under the health numbers.
- Name plates and unit-frame cast bars no longer show errors when the game keeps a plate's look or a cast target's size hidden.
- The addon memory tooltip on the info bar no longer leaves a mark on Blizzard's frames while it refreshes.
- Eldo-Vanilla: the enemy spotter moves down when the group pets grid is wide, so the two never overlap.

## [0.6.6004] - 2026-10-18

### New
- Eight new skins for the whole UI: Minimal Modern, Vanilla Original, Vanilla Refined, Warcraft Parchment, Forged Metal, Portrait Classic, Faction Heritage and Arcane. Each brings its own frames, buttons, bar texture, title font and accent color, and Faction Heritage follows your character's faction or the one you pick.
- The Appearance page under Layout and style: pick a skin for the whole UI or let each layout bring its own, a faction look, a skin per part, and the look of Blizzard's own windows. Art style is now called Skin.
- Blizzard's own windows (character, bags, spellbook, menus and more) can keep Blizzard's original look, match your skin, or follow what your layout was made for. Windows you set by hand keep your choice.
- Unit-frame graphics: give your unit frames Vanilla rings or Portrait Bars frames in your skin's materials, or keep the flat look. Party and raid frames take your skin's material and a fine edge without taking more room.
- Keybind setup shows a preview before any key changes: a keyboard with your movement keys, the three main bars with what each key is for and your class's spell for it, and short How to play notes.
- Three Eldo-Vanilla layouts in the original game's arrangement: portraits in the top left corner, a round minimap top right, the action bars along the bottom with the chat beside them. Compact fits 1080p screens, and Focus brings your frames closer to the center.
- Each layout brings the skin it was made for. A skin you pick yourself stays when you switch layouts.
- The Vanilla preset pack. Shared packs now carry the skin, faction look, unit-frame graphics and Blizzard windows.

### Improved
- Action buttons, bar backgrounds, the minimap frame, chat tabs and window headers take on your skin's frames, ring and colors. The five classic skins look as before.
- The bar texture can follow your skin, and window titles can use your skin's font.
- Keybind presets now bind only the main bars 1 to 3 (plain keys, Shift and Ctrl) and come in three choices: Classic movement (recommended), A/D strafe and Number row. Bar 4 and your other bars keep their keys, Character moves to the comma key when a preset uses C, and each preset can be undone in turn.
- The Large and Compact action bar styles now fit every layout: frames around the bars step aside while a bigger style is on.
- Larger micro menu and bag bar styles move into the bottom right corner instead of running into the bars.
- The healer role places its combat text and extra aura spots clear of the optional parts (data panels, extra bars, loot feed, toasts and more) in nearly every layout.
- Move mode sits next to Reload UI at the bottom of the options window, so the Modes in one row setting is no longer needed.
- The setup's Role step keeps your class line short (the full list is in its tooltip), and every setup page fits with Large text.
- The auction house's bottom tabs share one boxed look on a solid dark rail, with the open tab clearly marked.
- The Characters window lists your characters as two-line rows with class icon, level, zone and last login, and the open one highlighted.
- Switches, fold headers, side-rail buttons and selected list rows ease into their hover and selection colors (instant with Animations off).
- Bags: a search that finds nothing says "No matches" in the search box, while your items stay in place, dimmed. Clearing the search brings everything back to full brightness.
- With the minimap buttons skin, the calendar and the addon compartment sit on the same flat boxes as the tracking button.
- Objective counts in the quest tracker sit at the right end of their line in the accent color (Look > Counts on the right).
- An Info Bar panel docked on the minimap with its background off keeps outlined text so it stays readable, and the switch says so.
- The Ready Check Report closes when a pull countdown starts, so it no longer covers the countdown.
- Camp Helper panel rows and tooltip lines can be translated and follow the theme's text colors and sizes.

### Fixed
- One hit now shows one number over your target: while hit numbers on enemy plates are on, Blizzard's damage numbers over enemies step back unless you set them to Show.
- Blizzard's own nameplate pieces stay hidden under EldoUI plates, and a reused plate no longer keeps aura rows from its last unit. The Nameplates page says which plates show now.
- Shaman totem timers no longer end up in the chat window; they sit above the totem bar you see or on their own mover.
- Blizzard's own auction screens, title and Create Auction button no longer show through EldoUI's Shopping, Selling and Canceling pages, and come back as they were when you return to Buy, Sell or Auctions.
- Clearing the item on the auction house's Selling page clears its price, total, deposit and listing line, and a late price answer for an earlier item no longer fills them in; Rename and the other list buttons are no longer cut short.
- The Split Timer's texts are clear again: its panel no longer covers them, they update at once when you change the look, and with the panel off they keep an outline over the world.
- Two-line lists grow with Large text so their second line is never cut off.
- Tooltips keep their item quality color on the new skins.
- The setup comes back after a cinematic even when the game doesn't say it ended.
- Using the Talent Planner, sending a dungeon route or writing a quick note while that feature is off now says how to turn it on.

## [0.6.6003] - 2026-10-17

### New
- Mage Travel: one button lists the teleports and portals you know with your rune counts; click a row to cast it. It has its own spot next to the Consumable Bar in every layout.
- Blessing Plan: plan which blessing each paladin keeps up on each class, then send the plan to the group or post it in chat with one click.
- Class reminders for rogue poisons on each weapon, paladin seals and Righteous Fury, priest Divine Spirit and Shadow Protection, and druid Omen of Clarity. Warlocks can show their Soul Shard count on the mana bar.
- Mages get a mana gem button on the Consumable Bar with the gem's count and cooldown, and it can be bound to a key.
- The Talent Planner and Blizzard's talent window have Import build: paste a talent calculator link, a talent string, a loadout string or an EldoUI plan, see what it holds, and save it as a plan.
- Training lists what you can learn soon, with the level you need shown in red.
- Minimap buttons can sit on a slim rail along the left or right edge of the map, with a tooltip naming each one; the "Button rail" style sets it up in one click.
- Shift-click the experience or reputation bar for a small details window with experience, reputation and honor in folding sections.
- The Combat HUD page opens on an overview with one folding section per display and its current state.
- General > Modes in one row puts Move mode and Keybind mode under one Modes button in the options window's sidebar.

### Improved
- A bar or unit frame style that would run into another frame in your layout now says so in its row ("Too large for this layout") instead of overlapping it: the Large and Compact bar styles in most layouts, and the Portrait and Healer frame styles in Modern.
- Every layout now puts the micro menu along the bottom next to the bags, sized and arranged to fit that layout. A micro menu you moved yourself stays where you put it.
- A new character sees EldoUI's chat and action bars from the first login, before the setup is finished. The Blizzard UI step can still bring Blizzard's back.
- The setup's preset packs, layout pictures, chat preview and last page use the same cards as the options window and follow your art style.
- Hovers, selections, switches and tabs in the options window and the setup change with a short, soft fade. Turn off General > Animations to have every change at once.
- Long settings pages (Consumable Bar, Cooldown Manager) fold their sections with a click on the section line; folded sections stay folded, and a search or a settings link opens them.
- When another addon does one of EldoUI's jobs, EldoUI tells you with an alert that has a Choose button, instead of a chat line.
- When a command needs a module that is off, every module says it the same way, names the addon that holds it back if there is one, and offers the enable command as a click that puts it in your chat box.
- Class setups add form bars for druids, Taunt for warrior tanks, item and pet macros, counters by level and restock items without replacing your list; Aura Groups offers ready-made examples for your class that keep up with your newest rank.
- The Training window sits beside the spellbook as its own window. Resize it or drag it free, and it remembers its size and place.
- My Adventure uses larger text, trip cards show their full titles, raids and dungeons show their own pictures and are listed only once, and the German and French texts were corrected.
- Imports and copied talent paths in the Talent Planner confirm in the window, with Undo for a copied path, and talents you already learned keep their pick order number on Blizzard's talent window.
- The character window's stat sections fold with one click and stay folded; labels and values line up at every text size.
- The instance log, the Recently grouped list and the split timer use two-line rows and folding sections, with boxed Copy, Remove, Whisper, Invite and Add friend buttons.
- Quest tracker section headers sit centered between two thin accent lines, with a small arrow that folds the section.
- The bag and bank windows keep their tools (sort, bank, view, search all characters) on a slim icon rail at the side, and every section title folds with a click. Ctrl-click a rail button for the Bags options.
- Right-clicking a Consumable Bar button opens a small picker with each item's icon, quality color and how many you carry.
- Cooldown Manager lists a group's icons with their keys, with buttons to reorder or remove them and a side rail for a new group, move mode and keybind mode.
- The zone name, clock and coordinates on the minimap sit on small backing plates so they stay readable on bright maps and never run into each other.
- The import window shows the result of each click in the window itself and lists which parts of a bundle were not applied and why.
- The macro editor's text grows with Large text.

### Fixed
- Blizzard's own nameplate no longer reappears under the EldoUI nameplate when a mob enters combat, changes phase or is set up again by the game, and your target's selection glow no longer shows through.
- The setup now opens on a brand new character, also after the race intro cinematic, and comes back on the same step after any cinematic or movie.
- Healer combat text no longer covers the action bars in EldoClean, EldoWide and EldoSyntax, and the ping feed steps aside for it in EldoCookies.
- Data panels docked on a round minimap stay inside the circle and keep enough background to read over the map.
- The font picker and the look preview in the options window grow with Large text.
- List rows in EldoUI windows keep their height.

## [0.6.6002] - 2026-10-17

### New
- Minimap buttons: the game's event link button can be placed on a map corner or hidden.
- Combat Text: Forever's new combat text choices (shields on you, your shields on targets, effects on your target, effects on other targets).
- The level-up card shows the health, mana and stats the level gave.
- Pet and stance bars have a Fill order option, so an upright bar fills column by column. Imported upright pet and stance bars use it.
- The setup's Other addons step can place Guidelime's guide window at your layout's guide spot (it moves there after the next /reload).
- The Shopping List tracker has its own visibility settings and hides in combat by default.
- Express setup has a class setup for every class. Hunters get pet frames and Feed Pet warnings, warlocks armor, pet and Healthstone reminders with a Soul Shard counter, rogues combo points on the nameplate and a Flash Powder counter, warriors rage ticks and a Battle Shout reminder. Mages, priests, druids and paladins get buff reminders you click to cast and a self-cast macro, and mages the consumable bar with conjured food and water first. Every class gets its key spells on empty action slots for its role.
- Warrior spells go on the bar of the stance they are used in, and rogue openers on the stealth bar.
- Shared window parts for module windows: fold sections with a centered title, two-line list rows with class colors and small action buttons, slim icon rails, and a colored line under a window title.
- EldoUI notices the addons you already use for bags, bars, frames, chat and more, steps back where they do the same job, and lets you pick which one handles each job on the new Other addons page or with `/eui addons`.
- The setup has a step "Addons you already use" when EldoUI finds one: keep your addon or let EldoUI take the job. Nothing changes before Finish, and Finish names every addon it turns off.
- Unit Frames, Party and Raid, Nameplates, Class Resources, Auras, Action Bars, Cooldown Manager, Minimap, Bags, Tooltips, Alerts and Banners and Loot now start with a live preview that redraws as you change their settings.
- The Talent Planner shows your plan's pick order: a small number on each talent tells you which of your plan's points takes it first, also on Blizzard's talent window, and the talent's tooltip lists every point. Turn it off under Pick order numbers.

### Improved
- With the minimap kept and skinned, Forever's new header and tracking button art now goes flat too, and the tracking button shows a plain tracking icon.
- Auction house: weapons and armor show their required level, like Forever's own auction house, and row tooltips show random suffix stats such as "of the Bear".
- Ctrl-click opens the matching options on many more EldoUI frames: the waypoint arrow and coordinate box, timer bars, the fishing bar, chat list editors, the emoji button, Raid Tools, Party Quests, NPC dialog choices, tracker rows, the bag gold and currencies, and more. Item slots keep the game's own Ctrl-click.
- Ctrl-click on an alert opens the options of the module that raised it.
- Aura Groups remember which example filled a group, through edits and Copy look, and the example list shows each example's description.
- "Totem buffs on you" dims a step for each shaman in your party who is out of range, and fully when all of them are.
- The social window's ignore list gets the EldoUI skin.
- Friend cards in the social window show class-colored names and your notes, and offline friends are dimmed.
- On a crowded vertical Encounter Timeline, the name column shows how many names did not fit ("+N").
- Blocked actions in the error log now show where they came from: the addon, the call chain and, when the game can't name the function, the file and line that made the call.
- A setup you pause with a role preview showing now saves only what the preview changed. Logging out puts the preview's values back, and the role step shows your pick again next time.
- The micro menu on its own mover has a spot in every layout, two rows beside the buffs.
- The farming bar shares the flight bar's spot and steps aside while you are on a flight path.
- Data panels form one column under the first, and panels attached to the chat or minimap stack instead of covering each other. Panels on the chat now sit above it.
- Every Class Power style fits the layouts for every class, combo points included. A druid's mana runs inside the power bar by default.
- Main tanks move beside the raid when it grows tall.
- Data panels placed in the chat window or on the minimap now sit inside that frame. The chat text and the minimap icons make room, so nothing around them gets covered. The chat window holds three panels, the minimap two.
- Importing an EllesmereUI profile puts a full-width data bar on the main Info Bar (left, center and right as in EllesmereUI) instead of a separate panel. A second one fills the second info bar, stacked right against the first when both sit on the same edge.
- `/eui probe bg` keeps its last 20 reports in your saved settings, so one file after a few battlegrounds holds them all (`/eui probe bg clear` removes them).
- Druid form mana stays inside the power bar with the druid class details, clear of a detached power bar.
- EldoUI's windows draw a soft light edge in the Modern style, and their text stays crisp without an outline at every text outline setting (bars and frames keep the outline you pick).
- The chat's side buttons (Copy, Find, Errors) use the shared icon rail every EldoUI window now has.
- The options sidebar starts with four quick actions (Move mode, Keybind mode, Global settings and Profiles), and the Search features box is one key away with `/`. What's new and Errors moved to the foot of the sidebar, next to the version line.
- The general settings are now five hub pages (Global settings, Layout and style, Modules, Profiles, Lists and tags): one sidebar row each, their pages as tabs at the top, and a page's own tabs as a smaller row below. Left and Right switch tabs after a click in the window.
- The options footer is calmer: Reload UI counts the changes that wait for a reload and names them in its tooltip (the banner over the page is gone), and the Share menu sits next to the page search with a new Copy from profile for module pages.
- The options window groups every section's settings on its own card under a small label, with taller rows and on/off switches instead of check boxes; clicking a setting's name still switches it.
- Option tooltips open to the left when the window sits near the right edge of the screen.
- With Leatrix Plus, TradeSkillMaster, ElvUI or a bar addon, EldoUI steps back only for the parts both do, instead of turning a whole module off.

### Fixed
- Dalaran Sewer Key tracking checks whether you have the key without requiring you to finish the dungeon quest first. Its description explains that one key holder can open the gate for the group.
- Error reports now also leave out quoted text in the error message itself, such as a chat line or another player's name.
- A full-width Info Bar now stretches to the new screen width after a resolution or UI scale change.
- The "Instance difficulty" minimap button setting is gone, because Forever no longer shows that flag. The Mail setting now says "The new-mail icon."
- Cooldown Manager keybind text finds the rank of a spell that is actually on your bars.
- Combat Text: "Auras fading" is gone, because the game no longer offers it.
- Flat frame art on Blizzard's player and target frames fits the new bars, and turning it off takes effect without a reload.
- Ctrl-click on the weapon enchant icons opens Buffs and Debuffs > Enchants again, and the Weapon Enchants box's Options… goes straight to that setting.
- EldoUI's move boxes no longer cover Blizzard's Edit Mode window.
- Camp Helper shows the right tier for every Spirit object (all three banners, Spinning Wheel, Loom) and relearns objects it saved with the wrong tier.
- Camp Helper no longer treats cooking fires in the world as camps, and recognizes your campfire by name on every game language.
- Hiding the Quest Tracker box in move mode now hides the quest tracker and Questie's tracker, also after a reload and in combat.
- The error log no longer shows doubled brackets after a blocked function's name.
- The info bar style with two bars is grayed out where the layout has no room for it.
- Spell Efficiency: a value exactly halfway between two shown numbers now always rounds up, on Windows and Mac alike.
- Cooldown Manager keybind text shows on a spell when you keep a lower rank of it on your action bars.
- The "Second info bar" switch is grayed out in layouts with no free edge for it, like the Two bars style.
- The class setup page no longer pushes its two options off the page; the list of what it does scrolls.
- On the Eldo-Blizz layout the stance bar no longer covers the target's cast bar.
- Healer role on Eldo-Wide and Eldo-Syntax: the combat text box no longer covers Battle.net friend toasts.

## [0.6.6001] - 2026-10-16

### New
- Setup: four preset packs on the Welcome page, Modern, Classic, Healer and Minimal, each a whole UI with a miniature of its layout. Apply sets up every step with the pack in one click; Customize goes through the steps with the pack filled in.
- Share your look as a preset pack: the Share menu's "Export my look as a pack" makes a string with your layout, art style, accent and styles, and importing one puts that look on your current profile.
- Every layout now suggests a style for each part of the UI: unit frames, group frames, action bars, auras, minimap, info bar, class power, combat text and nameplates.
- Right-click Hide: right-click an EldoUI box such as the Camp panel, the Info Bar, a datatext panel, a counter, Party Quests or the coordinate box and choose Hide. It stays hidden, also after a reload, and is saved in your profile. Unit and group frames always keep the game's own right-click menu.
- A "Lock right-click" switch (in the move panel, next to Locked, and on the Hidden boxes page) makes EldoUI's boxes ignore right-click, so nothing is hidden by accident.
- A Hidden boxes page under Modules lists every box you hid, grouped like move mode, each with a switch to show it again, plus Show all. A module's page has a Show switch for each of its boxes; it is the same setting.
- Move mode: right-click any box for a menu titled with its name: Hide, Hide this box (until move mode ends), Lock, Reset position and Options…. Hidden pieces leave Combat mode and All frames; pick "Hidden" in the view list to see them dimmed and bring them back. The move panel's Hide button now hides the frame itself and reads Unhide for a hidden one.
- XP and Reputation Bars: with upright bars, "Value tag at fill end" shows each bar's percent in a small tag beside the bars, at the height the fill reaches, with a pointer in the bar's color, on the left or the right. Off by default; the options page shows a preview.
- Panel tint (Global settings > Textures): give the background of every EldoUI window and panel a subtle Midnight blue, Pine green, Wine red or Dusk violet tint, picked from sample cards and applied at once. Text stays exactly as readable as on the plain dark panels. The Modern, Blizzard and WoW Forever art styles take the tint; Classic and High contrast keep their own background.
- Frame shadows (Modern art style) get Shadow strength and Shadow size sliders.
- Shaman Totems: a totem bar for shamans. One button per element drops your picked totem, pointing at a button opens every totem you know for that element, and Drop All drops the whole set (with Call of the Elements once you know it). Each button shows its running totem's time, and the earth button lights up while you are feared and know Tremor Totem. Seven style presets, key bindings and a visibility rule.
- Shaman Totems: a cooldown bar with your shield and its charges, the weapon imbue on each hand, Totemic Recall, Reincarnation with your Ankh count and your shaman cooldowns, plus optional ready icons for key spells. Click an icon to cast it.
- Shaman Totems: up to eight totem loadouts. Right-click Drop All to switch, save, rename, delete or share one as a string; a switch during a fight waits until it ends. An optional rule switches the loadout when you enter a dungeon, raid or battleground.
- Shaman Totems: small squares on the party frames show who your totems reach, the totem tooltips name who they miss, and a mob's tooltip names the counter totem for the fear, poison or disease you saw it cast.
- Shaman Totems: a group plan for Mana Tide Totem and the resistance totems, sent to your group with one click, and a shaman column in the Ready Check Report with the totems and Ankhs each shaman carries.
- Shaman Totems: the cooldown bar starts with the spells for your role (healer, melee or caster), taken from the Role page or your talents. Tick spells yourself and your picks stay.
- Shaman Totems: a shaman group panel lists every shaman in your group with Mana Tide Totem, Reincarnation, Ankhs and their part of the plan. Other shamans' cooldowns show once they click Share mine. Open it from the options or by right-clicking Drop All.
- Ready Check Report: the shaman columns also show each shaman's shield, weapon imbues and mana.
- Aura Groups: the "Totem buffs on you" example dims while your party's shaman is out of range, as the game reports it.
- Reminders: shaman weapon imbue reminders for each hand, alerts when your shield or an imbue runs out (in the combat text lane during a fight), and an optional sound when your shield drops.
- Class setup: shamans get their totem bar, cooldown bar, reminders, a loadout for their role, key spells on empty action slots and a few macros in one step, and Revert puts it all back.
- Nameplates: two new example rules for totems, and Aura Groups has a "Totem buffs on you" example for every class. The friendly totem rule's tooltip names the friendly minion setting those plates need.
- Info Bar: your datatext panels can show as a **Dashboard**, a compact list with one row per value: an icon, the value and a thin bar for durability, bag space, tracked currencies toward their cap, the reputation you watch toward the next standing and your profession skills. Bars turn yellow, then red, before durability or bag space run out, and clicking a profession row opens that profession (not in combat). "Add a dashboard" on the Panels tab sets one up; the panel's visibility rules (in combat, in instances, on mouse over) work as for any panel, and the options show a preview with sample values.
- Quality of Life: a **flight view** for flight paths, off by default (Travel tab). While you fly, the interface fades and one calm panel shows where you fly to, the zone below you, the time left and the route, with buttons for the map, your bags, landing early and leaving the view. Landing, combat, a ready check, a queue invite or Exit brings everything back.
- Other addons: when EldoUI ships a newer version of an addon profile you imported, it asks once after login whether to update it; "Not now" waits for the next version. Profiles are only ever set up on your click and never in combat.
- Action Bars: a Fill order option per bar. Columns first fills each column before the next one, like an upright bar.
- Action Bars: "Show mouse-over bars together" (General tab). Hovering one bar set to Mouse over shows all of them. Off by default.

### Improved
- Setup: the Other addons step now lists Details!, RestedXP, BigWigs, Deadly Boss Mods and Questie when you have them, each with a ticked box that places its window in your layout. Untick one and EldoUI leaves that window where it is.
- Talent Planner: paste a talent loadout string from a talent calculator site and it becomes a plan for its class, like a calculator link. For calculator sites EldoUI can't read yet, the message now suggests their talent string or talent loadout string instead.
- Import: EllesmereUI strings now keep upright bars in their button order, carry over "show all mouse-over bars together", and turn data bars into datatext panels with their datatexts, size, place and visibility.
- Right-click Hide now also works on the XP and Reputation Bars, the Encounter Timeline icons and the Reminders icons.
- The boxes EldoUI keeps for Details!, RestedXP, Questie and the boss mods can be hidden from move mode and the Hidden boxes page, and the Integrations page has a switch for each. Only EldoUI's box goes; the addon's own window stays as that addon shows it.
- Ctrl-click opens the matching options from more places: the XP and Reputation Bars, the Encounter Timeline icons, alert toasts and alert cards, and the windows of Alts, Training, Talents, Macros, Raid Loot, the Instance Log, Dungeon Routes, the Profession Planner, the Ready Check Report, the Death Log, Game Settings, Finder and the Legacy Planner. A window's help button or title bar names it in its tooltip.
- Alert toasts and alert cards show a small tooltip that says what a click and a right-click do.
- Setup: the Role step shows the role you pick on your frames at once; Back, the Welcome page or closing the window puts it back.
- Setup: after an update that adds a setup step, EldoUI offers it once. "Show me" opens a short setup with only the new parts, and "Keep my setup" changes nothing.
- Setup: Express setup for shamans also puts key spells on empty action slots and adds the class macros while there is room. Your own actions and macros are never replaced, and the last page lists them with Revert this.
- Setup: the Other addons step says "Newer profile ready" when EldoUI has a newer profile than the one an addon got before.
- Layouts: on ultrawide screens the loot feed stays left of the boss frames (Cookies, Blizz, Dark, Cozy, Plates) and Hunter's threat meter and combat timer stay beside the center, clear of bar 7.
- Layouts: the counters, the Feed Pet button, the split timer and the possess bar have a free spot of their own in every layout. The possess bar takes the pet bar's place, the Feed Pet button sits beside the pet frame, and in most layouts the counters move to the top-left corner.
- Setup: every step has one main button, Apply and continue, with Back beside it and Skip as a plain link. The Styles step shows each pick on your frames at once, and Back or closing the window puts it back.
- Setup: styles too large for the picked layout are grayed out with the reason, in the setup and on each module's Styles options; with the Healer role the group frame size comes from the role and the Styles step says so.
- Setup: the last page before Finish shows one card per step with Change and Revert, and after Finish a placement check names frames that now cover each other, with "Use the layout's spot" and "Open move mode".
- Setup: "Back up my setup" on the Welcome page keeps a named copy of your profile, and after an update with new layouts or packs EldoUI offers them once, with "Keep my setup" as the first choice.
- Move mode: with test frames on, every frame shows its name once. A frame with a sample names itself; the box name moves to a small tab above the box while you point at it or select it, so it never covers icons. The move panel is no longer see-through.
- Ctrl-click an EldoUI icon or button to open its settings, scrolled to the matching row with a short highlight: Reminders icons (straight to "Click an icon to cast or use it" while it is off), Info Bar texts (Alt-click, as some texts use Ctrl-click themselves), counters, the Camp panel buttons, the minimap clock and addon button drawer, the chat side rail, the Journal's help button, cooldown row icons and weapon enchant icons. The tooltip says so. In combat the settings open once combat ends; action buttons, unit frames and other click-to-cast frames keep their clicks for the game.
- Settings: X and Y (and Width and Height, Offset X and Offset Y) always sit side by side on one row. On the Positions page, Anchor gets its own row above them.
- Edit Mode: the EldoUI panel beside Blizzard's Edit Mode has an "EldoUI options" button that opens EldoUI's Edit Mode settings (in combat, they open when combat ends).
- Edit Mode: when Blizzard's Edit Mode window sits too close to the left edge of the screen, the EldoUI move panel docks on its right instead, and moves along when you drag Edit Mode's window. The EldoUI panel beside Edit Mode never covers Edit Mode's window either, and its buttons stack with Large text.
- Move mode opens in Combat mode: only the frames of your everyday fight screen light up (unit and group frames, bars, cooldowns, combat text, boss timers, alerts, minimap and chat). Pick All frames or a group in the panel to see the rest; a module's own Move button opens right on its frame. Test frames now show real spell and item icons.
- Chat: Whispers, Loot and the other extra tabs now sit on the same line as General and Combat Log, and the chat's scroll bar and "jump to the newest line" arrow stay inside the chat panel instead of on its edge.
- Game Menu (Esc): the EldoUI and Journal buttons now sit inside the menu, right above AddOns, in the menu's own button look, and the menu's frame runs down around them.
- Importing an EllesmereUI profile now rebuilds it as a full EldoUI layout: every action bar gets the source's buttons, buttons per row, button size, direction and visibility (bars it hides are switched off, mouse-over bars fade in on hover), the pet and stance bars follow too, and unit frames, party and raid frames, chat, minimap, cooldown rows and resource bars take its sizes and show rules where EldoUI has the same setting. Sizes are converted from the source's UI scale. After the preview choose **Apply as a new layout** (a new profile) or **Change my current layout**; both can be undone, and neither runs in combat. The preview lists everything it can't import in plain words, and a profile made for another game version says what was skipped.
- Layouts: every layout now has an action bar setup of its own that matches its name, from Wide's single long row to Blizz's classic stacked bars and Heritage's short bar beside the main rows. Side bars that are not full hide their empty buttons, and the experience bar is as long as the bar row it sits under.
- Layouts: action bars 6 to 8, the loot feed, the zone toast and the vehicle seats have a spot of their own in every layout when you turn them on. Action bar 8 now comes as a 6 by 2 block like bars 6 and 7.
- Layouts: the pet bar, the stance and totem bars, the extra action button, the fishing bar and the Battle.net toasts no longer touch the action bars, the chat or the unit frames.
- Deadly Boss Mods: EldoUI's quiet setup now covers DBM's new trash and boss cast alerts in WoW: Forever dungeons and raids. They stay on, follow your target and skip channeled casts.
- Tooltip and cooldown icons: their shadow can keep its own strength and size ("Own shadow look"), apart from the Frame shadows sliders.
- Friends: when your friends list opens in the social window, the Ignore and Recently grouped tabs sit under that window too, and its search bar takes the EldoUI look.
- Encounter Timeline: on an upright bar, spell names line up in one column beside the bar, level with their icons, so names never run over the other lane or each other.

### Fixed
- Gathering: on clients in every language, herb and ore nodes now show the skill they need in their tooltip, and map pins saved under a translated name get their skill color and filter once you have hovered that kind of node.
- Buffs and Debuffs: right-clicking a weapon enchant icon (poison, oil, stone, shaman imbue) removes it, like on Blizzard's buff frame, instead of showing a "blocked from an action" message. The enchant icons now also show the game's own tooltip, time and charges.
- Setup: the line under each step's title no longer runs into the title.
- Combat Text: renaming a scroll area while move mode is open now updates its box name, and the "(locked)" note no longer disappears when you change a setting.
- Eldo-Modern: the extra action button no longer overlaps the loot toasts.
- Easy self buff and the Shaman totem bar now notice a weapon imbue you just cast, such as Rockbiter Weapon on a two-hand weapon, instead of still reporting no main-hand enchant.
- Layouts: a layout that turns an EldoUI action bar off no longer brings Blizzard's bar of the same number back.
- Layouts: cast bars no longer overlap the pet frame, the cooldown buff bars or other frames next to them; with the player power bar detached, the player cast bar moves down under it.
- Move mode: an action bar that is off no longer shows a column of test icons without a box around it.
- Layouts: in Eldo-Modern and Eldo-Compact the focus frame sits a little higher and further left, with the focus target above it, so the focus cast bar no longer touches the player frame with the Blizzard-like, Perl or Portrait unit frame styles. In Eldo-Modern, Eldo-Joe and Eldo-Syntax the loot toasts sit a little lower, clear of the target's cast bar with the bigger unit frame styles.
- Move mode: the boxes of the extra resource bars on their own movers now belong to Class Power, so they go away with the module turned off and their spots are part of a Class Power export.
- Move mode: a cooldown group or free cooldown icon that is turned off, or that the profile in use doesn't have, no longer leaves an empty box behind, and the setup's placement check no longer reports it.
- Game Menu (Esc): the EldoUI and Journal buttons now use the same font as the menu's other buttons.
- Setup: each step changes only what it is about, on top of your own settings. Frames you dragged stay where they are when the setup keeps your layout, applying a step twice or going Back and Next changes nothing more, a pick you made stays when you change the profile choice on the Welcome page, the Blizzard UI choices never turn off a switch you turned on, and the last page lists only what really changed.
- Setup: Express setup and clicking through every step now end the same way. Both turn on auto repair, junk selling and fast loot (the Convenience page says they start ticked and can be unticked), and repairs pay from your own gold unless you pick the guild bank.
- A Lua error when an EldoUI frame changed size while the game was logging out or reloading (seen with the Enemy Spotter).
- Encounter Timeline: timers close together no longer pile up on each other. Icons that would touch move to an upper and a lower lane (a little smaller on a thin bar) and keep that lane while they travel, the soonest is always drawn on top, and no icon slides out of the bar. The waiting stack keeps every number readable, and its "+N" chip sits beside the stack instead of on a countdown.
- XP and Reputation Bars: clicking the pet experience bar now opens your pet's page in the character window; it did nothing before.
- AI party followers in follower dungeons show their class color on unit frames, portraits, cast bars and class-colored name tags, like players.
- When the game shows your friends list in its social window, that window now gets the friends window's look and can be moved and scaled like it.
- Cooldown Manager: the keybind text now shows on spells with several ranks, also when the bar holds a higher rank than the one the cooldown names.
- Training: trainer levels and costs are up to date for druids, mages, paladins and shamans, including the newest talent rank spells.

## [0.6.6000] - 2026-10-15

### New
- **Talent Planner**: paste a Wowhead talent calculator link or a talent string (like 0505-3200-5) into the planner's Import box or after `/eui talents import`. You see the trees and points before it is saved as a plan, and a link EldoUI can't read says why, naming the site (Icy Veins, Mobalytics, seemeta, Guild Order and Zockify links can't be read yet). Nothing is learned.
- **Talent Planner**: plan any class, not only your own. Pick the class at the top of the planner; plans for other classes are saved for your whole account, and a character of that class is offered them at login. A shared plan of another class is saved for later instead of refused.
- **Level-up checklist**: one card when you level up lists your plan's talent point, new spell ranks at your trainer with their cost (ranks your plan doesn't need are marked), class quests that open, gear you can now wear and dungeons in reach. Every line is a link: a map pin to your trainer or the class quest, or the planner or the Journal. Learn learns that one rank; nothing else happens on its own. It is the only level-up card: the alert lane's level toast and the Journal's level moment stand back while it is on, and Fanfare's celebration still plays.
- Move mode: "Hide boxes" in the move panel hides every box, name, the grid and the panels so you see your real UI with its test frames; a small bar brings them back. Hold "Peek" (or Ctrl) to see the real UI only while you hold it.
- The EldoUI button under the Game Menu (Esc) opens the EldoUI settings; a right-click starts move mode.
- Camera: "Use the largest distance" sets the max camera distance to the furthest this game client allows, read from the game itself, and the distance shows in yards. New rows set the zoom speed and turn on ActionCam, an over-the-shoulder view whose offset eases in as you zoom out, with optional dynamic pitch. Turning a row off puts your own value back.
- Camera Situations: two new situations, "Your group in combat" and "Travel form", and the distance sliders reach as far as the client allows. `/eui cam` also shows the max distance, the client's limit and the camera settings EldoUI holds.
- Camera: while another camera addon that sets the camera distance is loaded, EldoUI leaves the max distance, zoom speed and ActionCam to it and says so on those rows and in `/eui cam`; Camera Situations stays off then.
- The Info Bar can fold to a small tab or hide: use the arrow at its right end, the Bar shown setting, `/eui infobar show | tab | hide` or a key binding. Hover the tab to see the bar, click it to open. Frames placed against the bar stay where they are.
- Addon memory sits next to latency on the Info Bar. Its tooltip lists the addons using the most memory, EldoUI's own share and, while the game's profiler runs, the addons using the most CPU; click to free unused memory. It updates only while you look at it.
- Bags: right-click a section's title (Junk, Reagents, a bag or your own category) to hide it; a hidden section folds to its title, and one click shows it again. Saved per character. Searching still finds items in hidden sections and opens them with a note, and hidden items still count and sell.
- Import reads bundles: paste several strings at once (EldoUI, EllesmereUI or ElvUI profiles, Edit Mode layouts and other addons' strings, one per line, each optionally under a name line such as "Details:"). The preview lists every part in plain words; tick the parts EldoUI applies. Strings for other addons get a Copy button, and anything unknown is skipped.
- Chat can fold a burst of guild "has joined", "has left", "has come online" and "has gone offline" lines into one line per kind; point at [all] to see every name. Friends keep their own lines unless you choose otherwise. Off by default, under Chat > Alerts and filters.
- Spell ranks: action buttons that still hold a lower rank of a spell you know light up, while the spellbook is open (default), always or never. Works on EldoUI's bars, Blizzard's bars, Bartender4, ElvUI and Dominos, and spots macros that show a lower rank too.
- A Check ranks button on the spellbook page lists every lower rank in chat (where it is, its rank and your highest rank) and lights those buttons up; right-click it to move them to your highest rank. `/eui rankcheck` does the same check from anywhere.
- A "Lower spell ranks" row on the Glows page sets the look of that highlight.

### Improved
- Battleground Timers: capture bars learn how long an assault takes on this game client, from the game's own timer or from an assault seen until the base turns, and use that time from then on (Darkspear Islands gets capture bars this way). Arathi Basin and Alterac Valley start from the usual 1 and 4 minutes.
- Battleground Timers: Alterac Valley mine owners show without any setup, and a mine changing hands no longer starts a capture bar.
- Battleground Timers: Warsong Gulch's Flag back bar lasts 20 seconds, and the Alterac Valley reminder names the rider commanders for ram and wolf hides.
- Move mode: "Show test frames" now fills every frame at once. Party and raid frames, main tanks and group pets show together, loot toasts join the loot rolls, and every frame with nothing to show yet (cast bars, cooldown rows, timers, alert and loot toasts, combat text, the pet and extra action bars and the rest) gets a sample in your current look until it has something real to show. Windows that only open on demand keep just their box.
- The settings sidebar is shorter and calmer: modules sit in eleven small groups (Unit Frames, Action Bars and Cooldowns, Combat Info and more) with one row per module, and the general pages are gathered under Global settings, Layout and style, Modules, Profiles, and Lists and tags. Click a group name to fold or unfold it; the group of the page you open unfolds by itself. A page's tabs now show only at the top of the page.
- The installer's chat step previews your tabs the way the chat panel draws them: flat boxes with the accent line under the open one.
- Every right-click and dropdown menu in EldoUI's windows, bars and map pins (Bags, Merchant, Mail, Raid Loot, Characters, Talents, Loot Guide, Dungeon Routes, Waypoints and the rest) opens in the one EldoUI menu look: your theme font, the accent check marks, Escape to close, and dropdowns that open right under their button.
- Click hints read the same everywhere: the window mover's drag, wheel and right-click hints, the hunter pet reminder's Revive Pet hint and older plugin datatext hints now use the white action word and gray text of every other EldoUI tooltip.
- The Snapshots restore window, the waypoint paste window and the simulator resize from the corner grip like every other EldoUI window, and open at the size you left them.
- Loot Guide: the corner grip now makes the window bigger or smaller and the pages follow; Ctrl+mouse wheel on the title bar zooms, like the other EldoUI windows.
- Training: the corner grip sets the window's Width and Height, so the size stays after a reload.
- Reset position on the Characters, Raid Loot, Hardcore, Ready Report and Instance Log windows also puts their size back.
- Loot Guide level and drop chance sliders and the talent planner's level guide apply when you let go, so the page redraws once instead of on every step.
- Edit Mode presets show a short line under each button saying what it does.
- Blizzard UI overview lists every category with how many parts EldoUI replaces, skins or leaves to Blizzard, with a button to each tab.
- Upgrade arrows and item scores stay ready while the game loads item data: only the item that arrived is worked out again, so bags, merchants and the Loot Guide no longer stutter during big item loads.
- The Loot Guide's World page is much lighter on zones with many rares: upgrade checks run once per draw, opening a card or loading item names no longer redraws the whole page, and rares on your minimap are only read while the page is open.
- Auction House full scans save their prices a few hundred per frame, so finishing a scan no longer freezes the game for a moment.
- Class quests in the Attunements tab show the level they open at, a short line on where they start and what they end with, and only the chains of your faction.
- Move mode's test frames also show sample reminders and the raid tools bar, and the reminders sample stays as long as the test frames are on.
- In Edit Mode, the EldoUI panel sits under EldoUI's move panel instead of beside Edit Mode's window, and its list of frames EldoUI places folds away and scrolls, so it never runs past the panel.
- A reminder's tooltip says where to turn on click-to-cast when it is off.
- My Adventure's where-next cards include the next step of your class quest chain, with a map pin button.
- The level-up page of My Adventure lists the Talent Planner's checklist (talent point, trainer, class quests and gear). While the planner's level-up reminder is on, only that one reminder pops up; the page stays in My Adventure.
- The Loot Guide's World page builds its rare cards and creature lines as you scroll, so zones with many creatures open faster.
- The flight route bar's track line and the Unit Frames preview's power bar use your theme and shared colors.
- EldoUI's windows (the options window, Characters, Raid Loot, the error log, the command list, editors and more) resize from the grip in its bottom-right corner, which lights up in the accent color under the pointer. The content follows the new size instead of being stretched, each window remembers its size, and Reset puts it back. On tabbed windows such as Characters or Raid Loot, Ctrl+mouse wheel on the title bar still zooms the whole window.
- Sliders apply when you let go: dragging moves only the slider and its number, so changing the text size, opacity and other heavy settings feels smooth again. A click, the mouse wheel or a typed value applies at once.
- Windows opened from another EldoUI window (Import a string, Export, a question) open in front of it and centered on it, stay in front when you click the window behind, and Escape closes the front one first.
- Options window: every label sits on one line beside a control of the same width, so dropdowns, sliders and text boxes line up in one column. A narrow window or Large text switches to one column instead of squeezing the labels, the page text under the title no longer runs into the tabs, and long group names in the left list wrap instead of being cut.
- The chat panel is redesigned: the tabs sit as flat boxes on the panel's edge with an accent underline on the open one, and Copy, Find and Errors move to a slim rail on the left side, so the tab row holds only tabs and tab names are no longer cut short.

### Fixed
- On light styles the on/off switches next to each module in the options and the sidebar's dividing line are visible again.
- Looking at a layout in the setup no longer forgets the frame positions saved for your role; Back brings them back.
- Battleground Timers: a flag capture between two score ticks no longer makes the expected winner bar count down twice as fast until the next tick.
- Battleground Timers: the expected winner bar stays hidden, without errors, when the game keeps the score widget's values private.
- Spellbook: with the book art hidden, spell names, ranks and category headers are drawn in your theme's text colors instead of dark ink, so they read on the dark window.
- Character window: stat section headers such as "Primary Attributes" fit their column with Large text and in long translations instead of being cut on both sides.
- Character window: section header bars, the plain model background and the gear set warning border follow your art style and theme colors.
- Nameplates: the name, level, debuffs and buffs each sit on their own row above the health bar, and the cast bar keeps a visible gap under it, in every nameplate style and at every UI scale.
- Calendar grid, emoji picker, merchant rows, dungeon map grid and Loot Guide dividers use the theme's divider and track colors; the class power health bar and group frame fallbacks use your shared colors.
- Closing the Auction House during a full scan keeps the prices read so far; the Full scan button says when the last scan was cut short.
- Closing the Auction House no longer causes a short freeze.
- An error when an alert card appeared while other alerts were on screen.
- Pet Care warns again when your pet food runs low after you restocked it, instead of only the first time.
- Camp Helper recognizes camp features and utility objects on every client language, not only English: tooltips, the features seen count and Announce use the names your game shows.
- Quality of Life: new hidden graphics settings under Sound and misc: always sharpen, icons over things you can use, and volume fog outdoors and indoors with its quality. Each row only shows when your game has that setting, and nothing changes until you pick a value.
- Quest Tracker: "Untrack all quests" on the General tab stops tracking every quest after a question. The quests stay in your log.
- Alts: a Plans column (in the Leveling style) and the character tooltip show the talent plans saved for each class; right-click a character to open them in the Talent Planner.
- A Lua error in combat ("arithmetic on a secret number value" in the game's backdrop code) from EldoUI's boxes on nameplates, aura icons and unit frames.
- Chat bubbles with the EldoUI skin are a clean flat box around the text: no stretched pieces of the game's bubble art and no pointer floating under the box.
- Chat messages stay inside the chat panel and no longer run up into the tab row.
- Every built-in layout was reworked so frames no longer cover each other in move mode, at 1080p, 1440p and ultrawide: the totem bar takes the stance bar's spot instead of covering the pet bar, the item cooldown row sits above the buffs row with room for a full row, the Tracking Bars box only shows while the bars use it, and the notices above your character (ready check, reminders, countdown, Fanfare text, prompts) each have their own place.
- The battleground map no longer reaches past the top of the screen and sits beside the RestedXP guide instead of on it.
- The threat meter and the combat timer have their own spot in every layout, with the timer right above the meter, clear of the target frame, the right chat panel and the extra action button.
- The death recap and the death log moved up a little, so the recap no longer covers the item cooldown row.
- The setup opens again on the first login of a new character, after the loading screen, and a loading screen while it is open no longer closes it.
- Setup steps keep what you already set: your picks and applied steps stay after closing the setup or a reload, "Recommended" on the Blizzard UI step keeps the switches you set yourself, and a full look no longer moves frames of a layout you kept or applied.
- With Large text, the setup's page titles and descriptions stay above the accent line, the Role and Blizzard UI cards grow with their text, and Large text (and the other switches on the Accessibility step) can be turned off again there, also after going back.
- In the Plates layout, the player frame's detached power bar no longer covers the cast bar.
- Unit frames set to draw above other frames no longer cover the game menu or popups: "High" is now the top layer, and frames saved at the old "Highest" layer draw as High.
- The setup no longer offers NPC Dialog on its Modules step, and "Turn all on" leaves it off: it stays off until you turn it on in its own options page.
- The setup's last page names each change once ("UI scale: auto" instead of "UI scale UI scale: auto"), and the setup window keeps one size from step to step.
- Clicking a layout in the setup during combat no longer applies it after the fight on whatever step is open by then, where Back could not undo it: the pick waits for Apply or Finish, like a layout click anywhere else.
- The setup's Layout step shows the whole description of the picked layout (or the one under the mouse) under the cards instead of cutting it short, and the Styles and Chat steps no longer cut or overlap their texts.

## [0.6.5002] - 2026-10-14

### New
- Express setup: one click on the first setup page applies EldoUI's recommended choices for every step, then shows what changed.
- Full looks: the Styles step of the setup has one-click cards that set the layout, art style, accent, font and fitting styles together, each with a small preview.
- The last setup page lists everything the setup changed, grouped, with "Revert this" to put any part back as it was.
- An error log window: `/eui errors` (or Errors in the options window) lists every caught error with its count and time, shows the full text ready to copy, and can show only this session or only EldoUI. It works with the Chat module on or off.
- Every entry in the error log has a Report button: it shows the error as a ready-to-paste bug report, without your character's name, realm, guild or chat text, plus a link to the bug form. EldoUI never sends anything by itself.
- Map Notes remembers the rares you meet: target or point at a rare outdoors and a pin marks where you stood, with its name and when you met it. Kept for all your characters; forget one from its pin, or all of them on the Map Notes page.
- The Mail, Merchant, Trade and Auction House windows join the Windows page: drag them, change their size with the mouse wheel and reset them like any other window. Your earlier window size is kept.
- Farming: a session history window lists every saved session per zone with gold, item value, XP, items per hour and corpses looted, with totals. Open it from the bar's right-click menu, the Info Bar text, the options page or `/eui farm history`.
- Alts: a Gold tab shows your gold over time, for one character or all of them added up, per day or per week.
- Pick the sound of the alert toasts and of the ready check and other pop-ups.

### Improved
- The Alts window (Guild and Crafters tabs), Raid Loot, the Loot Guide pages and the Restock list now show what a button did inside their window instead of in chat.
- Options buttons that delete or clear something now ask a clear question that says it can't be undone, and the questions for deleting a nameplate rule, a tracking bar or a Fanfare trigger no longer refer to the page behind the dialog.
- NPC Dialog leaves R to your Reply key by default; a new "R shows only the rewards" switch under Keys turns the rewards view key on, and Shift+R or Alt+R always reach the game.
- One Money style under Fonts and text sets how gold is written everywhere: bags, prices, trade, the Info Bar, tooltips and more. Bags, Auction House, Merchant and Trade can still keep their own choice, and letters no longer show empty silver or copper.
- The Import preview of ElvUI and EllesmereUI strings is written in plain words: frame names as those UIs show them, and positions like "bottom of the screen, 210 left and 180 up".
- With Large text, the Edit Mode position dialog and the EldoUI panel beside Edit Mode keep their title above the accent line.
- Tab moves to the next field in EldoUI's forms (Shift+Tab goes back): the Macro Editor's name and text, the Import window, map notes and the auction price boxes.
- Blizzard's Edit Mode now opens EldoUI's full move tools with it: the EldoUI move panel (search, exact X and Y, lock, attach, match size, test frames, undo) docks beside Edit Mode's window, every EldoUI frame can be dragged, and leaving Edit Mode leaves EldoUI's move mode too. When Blizzard's grid is shown, EldoUI's frames snap to it. Prefer the compact boxes? Turn off Full EldoUI move tools in the panel beside Edit Mode.
- Accent colors read better as text: with a dark accent such as Crimson or Violet, titles, active tabs, links and highlighted words use a lighter shade of the same color, while bars, lines and swatches keep the color you picked.
- Status colors are easier to tell apart with color blindness: the "good" green leans toward blue-green, and the good, warning and problem inks on parchment pages are teal, olive brown and wine.
- One "Copy settings from" button on every page with several frames of one kind: Unit Frames, Group Frames (each section), Nameplates (each plate type), Action Bars, Combat Text areas, Info Bar panels, Aura Groups and Tracking Bars. Before anything is copied, it shows which settings will change and asks to confirm; the on/off switch and the position stay as they are.
- Danger Alerts has six style presets (Standard, Quiet, Loud, Raid focus, Explorer, Barnyard) that pick the sounds, the flash and which alarms are on; your spell list stays as it is.
- Party Quests is on by default, and so is Sync with group: it shares your quest progress with group members who run EldoUI, as addon messages only, never in chat. It stays silent in battlegrounds and arenas, and in raids while Hide in raids is on.
- Chat guild mutes: when Decline their group invites or Decline their duels turns someone away, one chat line names who and which muted guild (both still off by default).
- Clearer page names in the settings: Character is now Character Panel, Characters is now Alts and Alerts and Messages is now Alerts and Banners. Your settings and `/eui` words stay the same, and the search still finds the old names.
- Windows: one Move Blizzard windows switch with a tick for each window under it. Ticking a window is all it takes; its Blizzard UI switch follows on its own. Your current choices carry over, and the mouse, scale, placing and fading settings moved to a Behavior tab.
- Tweaks is now part of Quality of Life: one page with Interface, Social, Quests, Travel and Sound and misc tabs. Every setting carries over; if one of the two was switched off, its features stay off. `/eui tweaks` still opens the page.
- Visibility settings: the separate instance options are now one "In instances" choice (Same as outside, Always shown, Fade, Hide or Only there). Your earlier choice carries over.
- Options window: the arrow keys and Enter move through the menu only after you click in it or in the search box. Otherwise they reach the game, so you can still move your character while the window is open.
- The Legacy Planner has the same keys as the options window: Ctrl+F puts the cursor in the Challenges search, and Esc clears the search before it closes the window. The keys only work out of combat, and every other key still reaches the game.
- XP and Reputation Bars, Raid Tools, the damage meter and the Cooldown Manager viewers now use the same Visibility settings as the rest of EldoUI (preset, Show, the extra rules behind the gear, faded opacity). Your Hide in combat, mouse-over and opacity choices carry over.
- Importing: one Import and export page with one paste box for every string (EldoUI, EllesmereUI, ElvUI and Edit Mode). It tells which kind you pasted and shows what it imports before you click Import. The separate "Import from other UIs" page is gone; its choices are on the same page.
- Layouts, boss fights: in every layout the boss frames, boss mod bars, Encounter Timeline and DBM info frame now form one tidy group right of the center. The timeline sits right under the boss mod bars with its big icon at the "now" end, the info frame no longer covers the special warnings, and the encounter power bar sits under the boss frames. Apply your layout again to get the new spots.
- Layouts, action bars: Eldo-Dark's bars form one even 2x2 block, Eldo-Plates and Eldo-Joe have full-size side wings that line up with the main bars, Eldo-Zen and Eldo-Hunter use one button size per block, and Eldo-Blizz's unit frames sit right on the visible bars.

- On WoW: Forever, new profiles start with the WoW Forever art style and the Sand accent. Existing profiles keep their look.
- Applying a keybind preset or importing another addon's profile now shows an alert with an Undo button.
- Keybind mode no longer writes to chat: the key you just set shows on its banner, and saving or discarding shows one short notice. Its tooltips follow your accent and text colors.
- Dragging a slider or picking a color on the General and Colors pages stays smooth: the UI updates once you stop.
- The options window measures EldoUI's memory when it opens or when you point at the line, instead of every two seconds.
- The options window builds its search in the background after it opens, so the first search no longer stalls the game.
- Every question EldoUI asks uses its own dialog look, and Esc cancels it.
- Tabs are flat everywhere, with an accent underline on the open tab, and hover highlights fade in and out softly (instantly with Animations off).
- The setup's step list and title match the options window.
- The Auction House window uses the same buttons, inputs, scroll bars, tabs and tooltips as the rest of EldoUI.
- The bag window's toolbar icons are calm gray glyphs that light up on hover, and "All" shows clearly when it is on.
- The Edit Mode position box, the waypoint entry, the link copy box, the message history window and the Training window use the same look as the rest of EldoUI.
- Tabbed EldoUI windows and the Loot Guide take Ctrl+F to their search, clear a search with Esc before Esc closes them, and switch tabs with Ctrl+Tab and Ctrl+Shift+Tab.
- Clearer module names: Alerts and Banners, Quest Marks (was New in Forever), Class Resources (was Player Power), Micro Menu and Bag Bar, and Fanfare (was Sound and Fun). The old names still find them in search and `/eui`.
- Clearer option names, such as "Show whispers only in the messenger", "Sell gray items at vendors", "Draw above other frames" and the Chat tab "Errors and help".
- Accent color toggles come with the style presets and sit under "More"; your own choice is kept.
- Window size rows say "Size" in percent, and windows with a corner grip no longer show a second size slider.
- Tabs in the Loot Guide, Legacy and Loot Simulator windows use the EldoUI tab font, and they follow Large text, as do the tooltip, quest tracker and chat bubble fonts. Buttons grow with their label, so Large text and translations never clip them.
- Skin switches ask for a reload only when you turn them off.
- Settings that need a Blizzard UI switch are grayed and name the switch to turn on.
- Buttons in the options window confirm inside the window instead of in chat, and so do style presets and layouts.
- One clock format and one pair of durability colors for all of EldoUI, on the General page. Your earlier choices carry over.
- One whisper sound, shared by Chat and Instant Messages.
- Every font picker shows each font in its own face and lists fonts from other addons.
- The minimap addon menu entry starts move mode; right-click starts keybind mode.
- `/eui help capture` lists every addon EldoUI can capture.
- Pet Care, Buff and Consumable Reminders and the low ammo warning show their notices as alert cards instead of chat lines.
- Loot Guide wishlist alerts can show as an alert card with a button that opens the item.
- Settings sharing and the version check wait politely when the game limits addon messages.
- Modules that read your bags share one read, so opening the bags or a vendor does less work.
- Player Notes texts in menus, tooltips and `/eui note` replies are translated.
- World bosses are labeled "World boss" on Map Notes pins and in the Loot Guide, and loot data marks every rare as rare, rare elite or world boss.
- The Loot Guide's dungeon entrance pins step aside where the world map already shows the game's own entrance pin.
- The "Show unexplored areas" option says plainly that an area shows once any of your characters has explored it.
- Party frames: buff and debuff positions can sit in one row under the frame, and the Perl party style uses it.
- Farming shows items per hour, and right-clicking the bar no longer resets the session without asking.
- Journal pace: the session pace takes over only after ten minutes with some XP gained, and milestone times show up to five levels ahead.
- Buttons and commands that delete or reset your work now ask first: triggers, themes, groups, bars, lists, ledgers, snapshots, layouts, presets, scales, style rules, waypoints and more.
- Settings that only work while another switch is on are grayed out with the reason, instead of looking active or vanishing.
- Sliders where 0 means something special say it in the value box ("Off", "Auto", "Never", "Full", "Instant", "No limit" and more).
- Mistyped words after /eui kb, layout, blizz, editmode, streamer, tracker, training, testframes, crosshair, cursor and threat get the command's help instead of doing something else; /eui scale accepts any case.
- Modules that are off answer their commands with the same hint, naming the Modules page and /eui enable.
- Blizzard UI switches and modules that need a reload use the settings window's reload banner.
- Dates in history, logs, snapshots and messages use the month name and your clock format.
- Style presets do exactly what their cards say (Quality of Life Minimal, Raid Tools, Trade, Raid Loot, Map Notes Treasure hunter).
- Clearer option texts for Camera situations, Cooldown Manager, the shared cooldown colors, Aura Groups and the timer bars.
- Social: "See-through window backgrounds" works whenever any window it styles is skinned.
- Guild attunement results can be cleared while sharing is off.
- Reminders' durability warning follows Worn gear and Low durability on the General page: yellow when your gear is worn, red when it is low. A warning level you picked in Reminders carries over.
- The font pickers of the Encounter Timeline, Macros, Battlegrounds and Combat Text follow the theme font like every other font picker. A font you picked stays.
- The Loot Guide's "Dungeon entrances on the world map" option says that its pins step aside where the game shows its own entrance.
- `/eui chatdebug` says on and off in the same short line as every other switch.
- My Adventure is spelled the same everywhere: tooltips, key bindings, commands and settings.
- The full look cards in the setup each say what makes them different: their art style and the accent they bring. The recommended one has a "Recommended" tag.
- The setup's sidebar shows each step's state as a mark (check, cross or dot) as well as a color, and its tooltip names the state.
- Searching "transparent", "see-through" or "clear" now finds the opacity settings.
- Questions that delete or reset something name the action on a red button instead of a plain "OK".
- A module whose settings or start failed says so on its page, in the sidebar and on the Modules page, with a button to the error log.
- Hardcore, Map Notes, Rare Scanner, Ready Check Report, Split Timer, Transport and Waypoints now open on their first real settings tab.
- Wiki: the commands page now lists every command, including Alts, Talent Planner, Legacy Planner, Instances, Macro Editor, Waypoints (`/way`), Rare Scanner and more.
- Warning numbers on the Info Bar (latency, durability, ammo, CPU, full quest log, full bags), the Ready Report and the character window's low durability carry a shape mark, so color is never the only sign.
- A currency at its cap gets a mark on the Info Bar, and its tooltip says whether it is the total or the weekly cap.
- The Talent Planner shows planned ranks as "learned>planned" and marks full talents (+) and ranks outside the plan (!), so they stay apart with any accent color.
- In the Instance Log, raids and battlegrounds that don't count are dimmed, say "not counted", and the tooltip says why.
- `/eui raidframes off`, `partyframes off` and `grid off` reach Party and Raid, and "Did you mean" suggestions also know module names.
- Pick a result in the Loot Guide's search drop-down with Up/Down (or Tab) and open it with Enter.
- Quality of Life hidden settings: each tick now says what it does ("Set my own combat text size"), so the page and the options search no longer show the same label twice.
- Enemy Spotter no longer sits right against the RestedXP guide or the party frames, and Eldo-Dark's cooldown bars no longer sit right against the focus frame.
- Menus in the options window and the move panel (select boxes, font and sound pickers, Copy from, the right-click row menu, Share, Group, Attach to, Match size) now share one EldoUI look, with the theme font, Large text, submenus to the side and a scroll bar for long lists.
- In-window notices stay while the pointer is on them or on their Undo button, and longer messages stay longer to read.
- Chat: the grayed name icon settings now say why they are off.
- Style presets: removed Tracking Bars "Plain", NPC Windows "Hunter" and Edit Mode "Strict", which looked the same as other presets. NPC Windows "EldoUI" now also turns instant quest text off again. Cooldown Manager "Fixed rows" now says it turns your own groups off.
- When the game's error window is hidden and the Chat Errors button can't show, EldoUI shows one notice per session when it logs a Lua error, with a button that opens the error log.
- Tracking Bars has a new Large text style preset.
- Escape now leaves move mode, like Done. While the move panel sits beside Blizzard's Edit Mode, Escape closes Edit Mode as usual.
- The Positions page now has one tab per frame group, like move mode. Frames of a module that is off stay listed, grayed out, with the reason.
- The move panel arrows, the attunement page arrows, Quick Menus' Back button and sub-menu marks, and the quest done and locked marks now use EldoUI's own icons instead of typed letters. The quest marks are drawn in their status color.
- Clearing the restock list, deleting a quick menu or a whole shopping list, and clearing a wishlist or the PvP planner now always ask first and show how many entries go. A hidden Shift-click is no longer needed, and the result shows in the window.
- Quick Menus shows its notices in its window while the window is open, instead of in chat.
- Large text now grows the labels of EldoUI's own buttons, and the buttons grow with them so no label is cut off.
- The EldoUI look on Blizzard's right-click and dropdown menus is now its own switch under Blizzard UI. Profiles that already skin Blizzard windows keep it.
- See-through panels and the lowest Panel opacity now stay at 80%, so gray and red text stays readable over a bright world. Text without an outline on see-through panels gets a soft shadow.
- Red warning text is a little lighter and green success text a little brighter, so they read better.
- The see-through switch has the same name on every settings page (See-through window, See-through windows or See-through background) and says where to set how see-through it is.
- Raid Loot's "Solid window" is now "See-through window", like everywhere else; your saved choice carries over.
- Spell Efficiency, the currency counts of your other characters and My Adventure's quest lines now sit in the tooltip's info area, under the divider, like every other EldoUI tooltip line. Choose when each shows on the Tooltip page.
- Spell Efficiency's "Show the line" choice moved to the Tooltip page (Spell efficiency); your saved choice carries over. New "Mana focus" style preset.
- The Errors entry in the options window shows how many new errors there are since you last opened the log.
- Dates and times everywhere in EldoUI follow the 12/24-hour clock setting and use the game's own month and weekday names in your client language. Dates from this year no longer show the year.
- Tooltip click hints read the same everywhere: one line per action ("Click: open the calendar"), in one hint color.
- The Gold datatext tooltip now mentions Shift-click for the Alts window.
- More tooltips name their clicks the same way ("Click: open it in the Journal"): Loot Guide rows, the Journal button, the item check line, the bank sort button, auction prices and the settings reset hint.
- The Loot Guide translations follow the new click hints and dates in German, French, Spanish, Portuguese, Russian, Korean and Chinese.

### Fixed
- "Hide duel results" no longer causes an error on every system message. Duel and drunk messages are hidden as intended.
- Enemy Spotter no longer errors on every update when a profile from an import or an older version lacks a size.
- Alerts and messages no longer error when the game locks one of its own frames that EldoUI scales.
- Tooltips hide the "Made by" and "Gift from" lines and the game's item level line at every item level.
- Item scores count enchants whose stat names have accented or non-Latin letters (German, French, Spanish, Portuguese, Italian, Russian, Korean, Chinese).
- Danger Alerts and the mailbox write counts like "1 spell" and "2 letters" instead of "spell(s)" and "letter(s)".
- The [threatcolor] text tag colors target frames and name plates by your threat on that unit.
- Spell Efficiency shows its tooltip lines on European English clients.
- Error reports remove character, realm and guild names with accented or non-Latin letters, and the base name on characters with a surname.
- With the Loot Guide off, My Adventure's commands and tour now say to turn on the Loot Guide, instead of pointing back to the My Adventure switch.
- The journal data check now points to the public Journal data report form, with its link.
- Pressing Escape on a question or a dropdown list now closes only that, and the options window and other EldoUI windows behind it stay open.
- With Large text, dialog titles no longer sit on the accent line under them.
- Short notices inside windows grow with their text, so notices of two or three lines, and Large text, stay inside their box.
- Raid Loot and the Dungeons window stay open in combat; other EldoUI windows that hide at a pull come back on the same page when combat ends, and a window you open in combat opens as soon as it ends.
- Snapshots keep macro names and the Cooldown Manager shows key binds for bar 1's second page even when the game's old action bar functions are turned off.
- Escape closes the AFK screen and brings the interface back, so the game menu no longer opens hidden behind it.
- Settings that point to another page now use the page names shown in the sidebar (Alerts and Banners, Camera Situations, Buff and Consumable Reminders).
- Party and Raid's Health text list now offers "Health current | %", so it shows correctly after the Perl style.
- The Cooldown Manager page now explains how to capture and import your own layout. Import waits until you have captured one, and names your class and spec.
- Importing a large gathering share no longer freezes the game.
- The Split Timer grows with Large text, so the time, the difference and the total never overlap.
- In the Quickdraw editor, the entry slots start under the help text, however many lines it takes.
- The zone name at the top of the minimap no longer runs into the clock. It fits between the corner items and ends in "..." when it is long, or moves one row down when there is no room.
- In move mode, the panel's help line stays inside the panel and above the controls, and the panel grows with Large text.
- The chat list windows (channel mutes, blocked phrases, alert words, guild mutes, chat colors, streamer aliases) and the Import window keep their help text above the controls with Large text, and list window titles are no longer cut.
- Chat: words joined by an ellipsis or a missing space ("wait...no", "nice.to meet you") no longer turn into web links; real addresses still do.
- The EldoUI panel beside Blizzard's Edit Mode keeps its text inside: long check box labels wrap and the panel grows with them, at every text size. Labels in Edit Mode's own check box columns that a larger game font pushed into the next column now fit their column while Edit Mode is open.
- Unit Frames and Buffs and Debuffs stop their background timers when switched off, and switching any module off stops every game event it listened to.
- A module whose settings fail to load after a profile switch, preset or theme change no longer stops the others.
- The Click-Cast Tips line under the click-binding window says off while another addon holds Click-Cast Tips off.
- The gear and sound buttons in the options window show a stand-in icon on clients that lack the game's art.
- Action bars read their slots through the current game API.
- The Edit Mode conflict panel closes with Escape.
- Tooltips no longer promise a right-click that does nothing.
- "Open the simulator" is grayed when the simulator is not installed, "Repair once you can afford it" while automatic repair is off, and "Ask for a camp" when you are not in the guild or group it would ask.
- Frames faded out by their Visibility rule no longer catch clicks meant for the game world or other windows. They take the mouse again as soon as they show, and "Mouse over" frames still answer the cursor. The Info Bar's Hearthstone button follows its bar the same way.
- Map Notes City services: mount vendors and stable masters no longer show as innkeepers.
- /eui modules works again, and "See what's new" on the update note opens the What's New page.
- /eui notify test with a lane name runs that preview instead of printing the usage text.
- Switching, copying or resetting a profile in combat, by command, the Profiles page or an import, waits until the fight ends.
- /eui in combat with the settings window open closes it, and it no longer closes again after the fight.
- Info Bar: a datatext picked in a slot after an empty slot now shows on the bar.
- "Idle opacity" now changes modules that already fade while idle.
- Undo in Recent changes no longer lists actions it can't take back, and copied settings can be undone.
- Copy, delete and "Set every module to" lists show "Choose..." instead of "nil".
- The Positions page lists frames that appear later, and a new anchor keeps the frame where it is.
- "Low durability" can no longer be set above "Worn gear", and the move-mode grid box keeps the Grid size slider's limits.
- Camera Situations: changing a setting while a situation is active no longer makes the camera forget your own distance.
- AFK screen: turning on Fade the interface, Slow camera turn or Show your character while the screen shows applies at once.
- /eui grouptest no longer shows test frames while Party and Raid is off, /eui alts off turns the module off, /eui fish log shows your zone's catch log, and /eui sound answers when the sound id is wrong.
- Bags: the mode lists no longer offer a Custom choice that does nothing.
- The panel behind the top-center widgets shows while only other UI widgets are hidden.
- Lowering the mail, recent recipient or message history limits drops the oldest entries right away.
- Quest text sizes below 8 points no longer make quest text unreadable.
- Name Plates: the combat width and height read in pixels, style rule opacity reads as a percent, and "Reset this type" keeps the type's on/off switch.
- Ping key bindings name the right settings page.
- Quality of Life: turning off "Show the volume panel" hides it, a panel you closed stays closed, and "Decline guild invites" no longer declines invites from friends.
- Raid Loot: "Solid window" changes an open window at once, and /eui raidloot clear accepts only sr or tmb and says what it cleared.
- Tooltip: Info area rows show when they differ from their default, and right-click resets them.
- Layouts: switching layouts no longer keeps the Encounter Timeline length of the layout you used before; every layout now sets its own.
- Command help and usage lines show every word again; choices like "lock | unlock | reset" no longer lose letters.
- Counts read right at 1 ("1 time", "1 character", "1 item") in the error log, Alts, the ready check report, Merchant, Bags and more.
- What's New and the update note now cover version 0.6.5001.
- Captions in capitals show umlauts, accents and Cyrillic letters correctly in every language.
- Skipping the Convenience step of the setup no longer turns on auto repair, junk selling or fast loot.
- On the setup's Other addons step, the Cooldown Manager row names your class instead of an internal code, and no longer looks like a warning when there is no layout for your class.
- Long summaries on the setup's Finish page and its list of changes wrap instead of being cut off; long module names on the Styles step wrap too.
- Highlighted words in the setup follow the accent color when a layout preview or a full look changes it.
- The options search finds settings by every word you type, in any order, and ignores capitals and accents in every language.
- Searching a common word like "color" now counts matches on every page, module pages included, with a "Show all" row for long pages.
- Hovering a cut page name in the options sidebar shows the full name, and with Large text the sidebar is wider.
- Name Plates and Edit Mode now point to the right Blizzard UI switches.
- Lists you shortened (Alts columns, Info Bar slots from a style preset) no longer grow back with extra or repeated entries after a login.
- Copying or importing one module's settings while module on/off is kept per character no longer switches that module on for your other characters.
- The map note editor asks before deleting a note, and Escape in a text box no longer closes the editor and loses what you typed.
- Long spell names on unit frame cast bars are cut with "..." before the cast time instead of running under it and past the bar.
- Shift-clicking an item into the Counters watch box works again, and shift-click links from EldoUI windows use the game's current chat link function.
- Info Bar texts that open bags, the map, the character window, the calendar or social windows now work in combat; clicks the game blocks in combat now say so.
- Party and raid frames keep their ready check, target border, raid marker and roster updates after you switch them off and on again.
- README: the module list now uses the in-game name Alerts and Banners.
- Docs: the FAQ, Layouts page and feature overview now name Shift + right-click as the way to put a frame back to its layout position in move mode.
- Docs: the plugin guide is now published, and links in the README, credits and wiki open the right pages, including on the wiki.
- `/way 45,2 63,8` with decimal commas now sets the waypoint at 45.2, 63.8 instead of the wrong place.
- "Remove all waypoints" in the arrow menu and "Remove all on this map" on the map pins now ask first, naming how many waypoints go.
- Deleting a journal backup in My Adventure now asks first.
- Clear in the chat panel's Errors tab now asks first, like the error window.
- In the Legacy Planner, Clear draft, Copy my build and Load into draft ask before replacing a draft that has ranks, and Overwrite asks before changing a profile shared by all your characters.
- Color-blind safe colors now also reach the Info Bar, the Instances counts, the Camp Helper and the options window's warnings.
- German clients no longer show an error on recipe tooltips or when an auction sells, and the "Auction sold" alert plays again.
- "Hide other players' crafting" now works on German clients.
- The Hardcore death log on Portuguese clients names the right victim and killer.
- Lowercase searches now find Russian and accented names in bags, the whisper history, the mail log, the death log, the reminder picker, move mode, waypoint zone names, the Legacy Planner and the Loot Guide pages.
- Shortened names and labels (reputation on the Info Bar, journal notes, saved names, chat lines) no longer cut a letter in half in Russian, Chinese or accented text.
- Raid Loot JSON imports keep accented and non-Latin letters instead of turning them into "?".
- My Adventure counts kills on every client language, also at the level cap.
- The Ready Check Report and the Macro Editor no longer show a single tab that does nothing.
- The Ready Check Report shows its summary once, and it wraps with Large text instead of being cut.
- My Adventure's level river shows the name of every part, including the newest one at level 60.
- Setup cards (such as "Guild bank first" and the fresh profile) grow to show their whole description, also with Large text.
- The ping feed's time and sender columns follow the text size, and senders show without their realm.
- In party and raid frames, aura and defensive icons no longer cover the name and health text.
- With Large text, option dropdowns are wide enough for their choices and long page titles fit the header.
- The Macro Editor's empty-list hint wraps inside the list instead of being cut at both ends.
- The error log's privacy note wraps under the detail box and reads in full at every size.
- The Loot Guide's first-run card shows each choice's whole description.
- "Whisper your target" whispers players with a surname correctly instead of a non-existent "Name-Surname".
- Dungeon run stats save group members by their name, not as "Name-Surname".
- With a surname, your own messages are no longer treated as someone else's: you no longer show as typing to yourself, get a Party Quests card for yourself or invite yourself from chat, and your own settings offers and guild attunement progress are recognized.
- `/eui <module> off` works with the module's name as the config window shows it, for example `/eui party and raid off` or `/eui loot guide off`.
- A module whose name is also a command switches with `/eui <name> off` (Chat, Edit Mode, Quickdraw, Raid Tools, Raid Loot and others), and the module list in the wiki names a word that reaches every module.
- The Loot Simulator now uses an item's stats as soon as the game has them, instead of showing "no numbers yet" until a reload.
- The Loot Simulator now uses your real weapon skill, including racial and gear bonuses. When the game doesn't show it, the result page says the simulator used the usual skill for your level.
- The Loot Simulator now counts your talents, a talent change marks saved results as outdated, and the BiS export lists your talent points.
- Rating a two-handed weapon no longer counts your off-hand item's stats.
- A page's short tour no longer opens on top of the Loot Guide's welcome card; it shows on a later visit.
- The Crafting empty text, the PvP planner line and the BiS help text now wrap instead of being cut off.
- Tooltip "Hide in combat" now hides every tooltip for its mode: "Over UI frames" also hides spell, aura and EldoUI frame tooltips, and "Over the world" hides herbs, chests and other world objects.
- Tooltip "Hide in combat" and "Hold to show in combat" are grayed out and name the Blizzard UI switch Tooltips: Hide they need.
- The end of a long fight no longer stalls while the same refresh runs once for every event seen in combat.
- Leaving the WoW Forever art style on the General page now gives back the layout's own accent instead of blue.
- Switching between layout presets no longer keeps settings the previous preset set, such as target plate details, bar shapes and Info Bar texts.
- Hardcore's death log no longer covers the death recap.
- In Eldo-Zerby the Cooldown Manager's Mobility group no longer covers the focus frame.
- Cast bars, the crosshair range tint, Fanfare texts and many smaller places now check for hidden game values before comparing them, so they no longer error when the game restricts a value.
- Name Plates: removed the "Raid marker" style filter condition and its "Skull: red border" example. The game never shares raid markers with addons, so they could never match. Your other rule conditions keep working.
- With "Blizzard's own UI" or "Only EldoUI's own frames" picked in the setup, Blizzard's menus keep their own look.
- The EldoUI datatext showed its click hints in white instead of the hint gray.
- Hardcore window times used a fixed US 12-hour format.
- Quick Menus deletes the menu its question named, even if you pick another menu while the question is open.
- With Large text and the 12-hour clock, the times in the error log are no longer cut off.

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

[Unreleased]: https://github.com/Eldodeldo/EldoUI/compare/v0.6.6004...HEAD
[0.6.6004]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6004
[0.6.6003]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6003
[0.6.6002]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6002
[0.6.6001]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6001
[0.6.6000]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6000
[0.6.5002]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.5002
[0.5.0]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.5.0
