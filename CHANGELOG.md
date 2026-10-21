# Changelog

All notable changes to EldoUI, newest first. Each version starts with its highlights, then what is new, what was improved and what was fixed. Every line names the part of the UI it touches, and changes for one class carry the class name. Versions are listed as `[version] - date`.

The in-game **What's New** page (`/eui whatsnew`) shows the highlights of each version.

## [Unreleased]

### Fixed
- **General:** Every EldoUI version can be downloaded as a zip from its release page.

## [0.7.0000] - 2026-10-21

### Highlights
- Ten built-in layouts with clearer names, and EldoUI Center as the new default for new profiles.
- Four roles in the setup and on the Role page: Melee, Ranged, Healer and Tank.
- A new Keys and spells step shows your keys, class spells and macros first and changes nothing on your bars until you press Apply.
- With the Vanilla Original skin, the unit frames, the action bar tray, the minimap border and the micro menu wear the game's own classic art.
- Every layout or pack change can be undone, from the alert after the change or with /eui layout undo.
- Your settings, layout, dragged frames and journal carry over to this version, and a copy is kept first that the new Saved data page can put back.
- EldoUI's own texts are now available in Danish, under General > EldoUI language.
- Nameplates, bags, cooldown displays and many other parts do much less work, and background work pauses in combat.

### New
- **Setup and layouts:** Ten built-in layouts, each with its own shape on screen: Vanilla Original, EldoUI Center, Modern Center, Blizzard Bottom Block, Portrait Staggered, Compact HUD, Widescreen Edges, Close Combat, Open Center and Nameplate Focus.
- **Setup and layouts:** EldoUI Center is the new default for new profiles: player and target sit level with the cooldown row, and the action bars form one block at the bottom with a narrow wing on each side. Profiles from earlier versions keep the layout they used.
- **Setup and layouts:** Four roles in the setup and on the Role page: Melee, Ranged, Healer and Tank. Ranged also shows the five-second rule on your mana bar.
- **Setup and layouts:** Every layout or pack change can be undone: press Undo on the alert after the change, or type /eui layout undo. Settings you changed yourself since stay as you set them.
- **Setup and layouts:** A new Keys and spells step, also on Express, shows your key preset, class spells, macros and rank upgrades before anything changes. Your bars change only when you press Apply, your own actions, macros, items and kept ranks stay, and one Undo puts it all back.
- **Setup and layouts:** In move mode, the pet and stance bars can be laid out Horizontal, Vertical or as a Grid, and the action bars, pet and stance bars, micro menu and bag bar have Size and Spacing menus.
- **Setup and layouts:** Move mode's frames menu has Find a frame: pick any frame to show, select and flash its box, and bring a frame that ended up off the screen back to the nearest edge.
- **Unit frames:** A new Classic frames style gives the player, target, target of target and pet frames the shape of the original frames, with a round portrait.
- **Unit frames:** With the Vanilla Original skin, frames sized like the originals wear the game's own classic frame art, with the elite and rare dragons on the target. The Vanilla Original layout shows them as soon as you pick it.
- **Action bars:** With the Vanilla Original skin, a one-row bar 1 sits on the classic stone tray with a gryphon at each end, the stance bar gets its classic stone, and the micro menu and bag slots wear their classic buttons.
- **Journal:** My Adventure keeps every dungeon and raid run with who was in it (name, class, level and role) and its loot rolls: who won which item and everyone's roll. Battlegrounds and arenas record nothing.
- **Journal:** Delete one run or one name from My Adventure with Undo. EldoUI never drops runs or companions on its own, and companion pages show what each companion won while grouped with you.
- **Map and minimap:** The Vanilla Original skin puts the game's own classic border around a round minimap, scaled with the map.
- **Saved settings:** Every update first keeps a copy of your settings and journal. The new Saved data page (or /eui data) puts a copy back, lists what a restore replaced so one click undoes it, and keeps any saved value EldoUI could not read aside instead of deleting it.
- **Localization:** EldoUI's own texts are available in Danish: pick Dansk under General > EldoUI language and reload. Game words players say in English, such as quest, loot and raid, stay English.
- **Localization:** The setup's first step lets you pick EldoUI's language, with the same flags as General > EldoUI language, and offers the reload right away.
- **General:** Mage Travel, the Party Quests panel, the Split Timer and the waypoint arrow can be set to show only in combat, out of combat, on mouse over or in a group, like the other HUD pieces.
- **General:** /eui probe textures lists which original interface textures your game client ships, ready to copy into a bug report.
- **Mage:** Mage Travel has five style presets: Standard, Small, Large, Quiet and Out of combat.

### Improved
- **Setup and layouts:** Picking a layout gives the same result from the Layouts page, /eui layout, the Overview, a pack and the setup: the layout's skin, Blizzard windows and suggested styles, nameplates included.
- **Setup and layouts:** Frames you dragged stay where you put them when you change layouts, unless you tick "Put frames I dragged back in the layout's spots". Applying the layout and look you already use changes nothing.
- **Setup and layouts:** If you picked a skin yourself, choosing a layout asks once whether to use the layout's look; "Keep my look" is the default.
- **Setup and layouts:** Layouts that left the list stay as legacy layouts, so your screen does not change after the update. If you had moved frames, a copy of your screen is also saved under your own layouts.
- **Setup and layouts:** One layout picker on the Layouts page, the Overview and the move panel: the ten layouts first, then legacy layouts you still use, then your own. The Overview and move mode show your layout, role, skin and Blizzard windows.
- **Localization:** General > EldoUI language shows each language's flag. The Danish texts come in a folder of their own that loads only when you pick Dansk, so playing in English uses no extra memory for them.
- **Localization:** With Dansk picked, menus, lists and window titles that still showed English now show Danish too, and so do the What's New page and the update note.
- **Setup and layouts:** A profile that used the older Damage role moves to your class's Melee or Ranged role by itself, and every frame stays where it was.
- **Setup and layouts:** The setup waits while the game asks whether to skip the intro cinematic, and while Details! or Questie show their own first-start windows, and opens once you have answered.
- **Setup and layouts:** The Other addons step in the setup lists only the addons EldoUI has a profile ready for, for your layout or specialization.
- **Unit frames:** A unit frame graphics choice that does not fit your layout is grayed out, with the reason in its tooltip.
- **Unit frames:** The unit and party frame style with the boxed 3D portrait and name bar is now called Boxed.
- **Group frames:** Party and raid frames keep the empty part of the health bar dark and clearly apart from the frame art in every skin, and the Minimal party style shows a slim mana bar on healers.
- **Nameplates:** Nameplates do much less work in big groups and cities: each plate listens only to its own unit, cast bars and hover update only while there is something to show, and quest progress and NPC titles are read once per change.
- **Nameplates:** EldoUI's nameplates wear your skin's frame edge, the same thin edge as small unit frames, and follow your unit frame graphics choice. Target, focus and style rule border colors still come first.
- **Action bars:** The class setup puts each key spell on the button of its keybind category, now including Shield Wall, Hammer of Justice, Freezing Trap, Frost Nova and Ice Block.
- **Action bars:** Cooldown rows show the key of another rank of a spell when that rank is on your bars, and spell buttons on the Consumable Bar, mounts included, show their cooldown without a global cooldown swipe.
- **Talents and spells:** The Planner row on Blizzard's talent window stays inside the window on small screens, and the Talent Planner tells you when Improve for Spellbook and talents is off.
- **Tooltips:** On the Tooltip page, a row whose module or switch is off is grayed and says why.
- **Journal:** Long run lists open one page of 100 runs at a time, and a journal with years of runs opens as fast as a new one. Runs and the people you ran with take about half the saved space, with nothing lost.
- **Map and minimap:** Show unexplored areas works from your first login: the parts of every zone you have not explored yet show dimmed, even where none of your characters has been.
- **Windows and skins:** Turning a window skin or the Mail module off puts Blizzard's look back at once, without a reload: spellbook, professions, quest and gossip dialogs, mailbox, friends, guild, calendar, PvP, the game menu and addon option windows.
- **Windows and skins:** Option gear panels, the Recent changes list, the setup's questions and help, the dungeon map and the journal's quick note share the look of EldoUI's other windows, and Escape closes the front one first.
- **Windows and skins:** Text sizes, tooltip titles and tooltip text match the rest of the interface in every window.
- **Notifications:** Alerts, the zone toast, rare cards and the low-mana note on a ready check share one queue: they no longer pile up, a repeated alert shows once, and alerts that waited out a long fight drop away.
- **Options:** Turning a module off or switching profiles asks for a reload only when a module really needs one, naming only the Blizzard parts that do. Switching a module on and off during a fight switches it once, after the fight.
- **Performance:** Bags, the vendor, the auction house, loot rolls, the Encounter Timeline, the Farming bar, Enemy Spotter, gathering pins and map coordinates redraw only what changed, and their timers run only while something is on screen.
- **Performance:** Cooldown rows, tracking bars, the cooldown pulse, the cursor ring, the Consumable Bar and the global cooldown bar share one cooldown reader, so a burst of cooldown changes redraws them once.
- **Performance:** Countdown bars, the ping feed, buff reminders, weapon enchant timers, minimap note pins, the quest tracker, waypoints, the Split Timer, Quickdraw and ActionCam work only while they show or are in use. Background work pauses in combat.
- **Performance:** The Loot Guide and waypoint arrows work out map positions with much less memory churn, Loot Guide search and the PvP page open faster, and the Loot Guide's side list waits until you open the window.
- **Performance:** Backups of a long journal and of years of runs are written a little at a time, so logging in after an update stays smooth.
- **Saved settings:** EldoUI records which version saved your settings. After an update every profile is brought forward without removing anything, settings you never changed keep the value you saw, and one chat line tells you.
- **Localization:** A name font you pick no longer replaces the font of Cyrillic, Korean or Chinese names, and name fonts stay in place when you change the theme font.
- **Localization:** The newest Loot Guide texts, such as run backups and loot rolls, are translated into German, French, Spanish, Portuguese, Russian, Korean and both kinds of Chinese.
- **General:** Changes EldoUI makes to Questie, RestedXP or Guidelime settings ask first, name the profile and the characters that share it, and can be undone. RestedXP's new guide window is placed on the layout's guide spot with its step list.
- **Shaman:** Totem timers kept with the totem bar move under or beside it when the cooldown rows fill the space above it, and tick only while a totem is out or an imbue runs.

### Fixed
- **Setup and layouts:** A profile that names a layout that is not installed now says so once and keeps your saved layout choice.
- **Setup and layouts:** A pack applied from the Overview or a pack string now also sets its role, and choosing the Healer pack after another pack no longer leaves raid frames covering your own frame.
- **Setup and layouts:** A micro menu or bag bar you moved in an older version stays where you put it, and the bar and macro check boxes on the class setup page remember your choice.
- **Unit frames:** Cast bars no longer show an error when an enemy casts something whose details the game keeps hidden, and keep the EldoUI look.
- **Unit frames:** Turning Unit Frames off brings Blizzard's own unit frames back at once, without a reload, unless they were set to be replaced.
- **Group frames:** With the Healer role, raids that use the Mid or Large raid settings keep the larger healer frames too.
- **Nameplates:** Turning off EldoUI's plate size after changing Blizzard's nameplate scale gives back the size the game uses now.
- **Action bars:** The zone ability's options, its box in move mode and its Blizzard UI switch name only the zone ability, and keybind mode no longer offers a key for an extra action button, which WoW: Forever does not have.
- **Talents and spells:** The Talent Planner, the Training tab and the spellbook skin go on and off together, whatever order you turn them on in.
- **Talents and spells:** With the game's gamepad interface on, EldoUI's buttons on the talent window, the spellbook and the trainer window step aside, and they come back when you switch to mouse and keyboard.
- **Tooltips:** Hovering an aura on an enemy nameplate in combat no longer causes an error with the smart tooltip position.
- **Journal:** Forgetting a character in the Alts window backs up its journal first and says so, and the newest backup of your runs from before an update is no longer pushed out by later restores or imports.
- **Journal:** The Attunements tab no longer lists WoW: Forever dungeons without a quest chain as empty pages; such a dungeon shows up once you have taken one of its quests.
- **Journal:** On a German client, quest objectives in the Loot Guide show in German.
- **Map and minimap:** Corner buttons on a small minimap no longer overlap.
- **Windows and skins:** Switching profiles or themes shows the new colors and skin right away, without a reload.
- **Options:** While the quest tracker is hidden by its Hide switch or its box, its visibility settings are grayed out and say why.
- **General:** Game windows, tooltips, nameplates, chat bubbles, the Training window and the Cooldown Manager no longer cause an error when the game hides a frame's layer or state from addons.
- **General:** Frames that fade out no longer cause an error when the game hides one of their parts from addons.
- **General:** Camp Helper recognizes every camp feature, the Anarchist's Workbench, Cookie's Feast and Iron Oven in any game language the first time you see them.
- **General:** The Durability info text shows its repair icon again.
- **General:** The camera no longer swings back and forth when you close one NPC window and open the next.
- **Paladin:** The blessing reminder, the Blessing Plan and the ready check report count only the blessings that share the blessing slot on WoW: Forever, so Salvation no longer counts as one, and Blessing of Sanctuary and Sanctity Aura are gone.
- **Shaman:** Water Shield and Rage of the Farseer work on the cooldown bar, the shield reminder and the class setup, Fire Nova has a ready icon, and Windfury and Flametongue Totem show on the party squares.
- **Shaman:** The totems and Earth Shield that WoW: Forever removed are gone from the pickers, and a saved pick of one goes back to the first one you know.

## [0.6.6005] - 2026-10-18

The versions from 0.5.0 to 0.6.6005 in short: what they brought that is still in EldoUI.

- **Setup and layouts:** A step-by-step setup with Express, a class setup for every class, a last page with "Revert this" for each change, and a once-per-login reminder for an unfinished setup.
- **Setup and layouts:** Preset packs (Modern, Classic, Vanilla, Healer and Minimal), UI amount (Essential, Moderate or Full), the Overview page with complete looks, and look strings to share.
- **Setup and layouts:** Move any frame with /eui move, hide a box with a right-click (a "Lock right-click" switch and a Hidden boxes page bring it back), and set keys with /eui kb.
- **Setup and layouts:** Imports of EllesmereUI, ElvUI and Edit Mode strings, and an ultrawide safe area.
- **Unit frames:** Unit frames with Blizzard element switches, heal prediction, text tags and cast bar effects, unit-frame graphics (Vanilla rings, Portrait Bars or the flat look), and a class resource bar with the five-second rule.
- **Group frames:** Party and raid frames with main tanks, group pets, raid sizes and click casting.
- **Action bars:** Eight action bars plus pet and stance bars, with fade and visibility rules, Fill order, proc glow and Masque, and keybind presets with a preview before any key changes.
- **Talents and spells:** The Talent Planner with Import build, pick order and a level-up checklist, Training with what your trainer teaches now and soon, and lower spell ranks lit on your bars, with Check ranks on the spellbook and /eui rankcheck.
- **Chat:** Saved history, search, keyword alerts, a spam filter, per-channel colors, and guild roster lines folded into one.
- **Tooltips:** Spell tooltips can show damage or healing per second and per mana, and the target or focus cast bar shows the spell's tooltip.
- **Bags and loot:** Bags and bank with your other characters' items and sections you can fold, merchant restock lists, the Loot Guide with best-in-slot sets and a wishlist, Raid Loot, Appearances and Farming history.
- **Journal:** My Adventure, a journal of your road from 1 to 60 told as a story, with backups and exports, and Attunements with raid keys, dungeon chains and class quests.
- **Map and minimap:** Dungeon Routes, Map Notes with the rares you met, Transport Maps, addon minimap buttons gathered behind one button, and a slim button rail.
- **Windows and skins:** Eight skins for the whole UI (Minimal Modern, Vanilla Original, Vanilla Refined, Warcraft Parchment, Forged Metal, Portrait Classic, Faction Heritage and Arcane), the Appearance page, panel tint, and skins for Blizzard's own windows.
- **Notifications:** Alert toasts with your choice of sound, the level-up card, the Ready Check Report and class reminders.
- **Options:** The Blizzard UI page with one switch per part of Blizzard's UI, the Visibility page with HUD presets, Recent changes with Undo, profiles that follow your character, talent group or content, and Large text, a High contrast skin, color-blind safe colors and sound cues.
- **Localization:** The Loot Guide in German, French, Spanish, Brazilian Portuguese, Russian, Korean and Chinese, and player names in Cyrillic, Korean and Chinese show their letters.
- **General:** The Info Bar with datatexts and a Dashboard, the error log (/eui errors) with a Report button that leaves out your character's name, realm, guild and chat text, Rare Scanner, the Encounter Timeline, Raid Tools with /eui pull, Combat Text and the Cooldown Manager.
- **General:** The Profession Planner, Finder, Macro Editor, Fishing, Streamer Mode, the Split Timer and Hardcore death alerts.
- **Mage:** Mage Travel lists the teleports and portals you know, and a mana gem button joins the Consumable Bar.
- **Paladin:** The Blessing Plan (/eui blessings) plans which blessing each paladin keeps up on each class.
- **Shaman:** Shaman Totems: a totem bar, a cooldown bar with your shield, weapon imbues, Reincarnation and Ankhs, up to eight totem loadouts, and a group plan for Mana Tide Totem and the resistance totems.

[Unreleased]: https://github.com/Eldodeldo/EldoUI/compare/v0.7.0000...HEAD
[0.7.0000]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0000
[0.6.6005]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6005
