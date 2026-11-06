# Changelog

All notable changes to EldoUI, newest first. Each version starts with its highlights, then lists its changes by the part of EldoUI they touch, with what is new, what was improved and what was fixed in each part. Changes for one class sit under Classes with the class name. Versions are listed as `[version] - date`.

The in-game **What's New** page (`/eui whatsnew`) shows the highlights of each version.

## [Unreleased]

### New
- **Nameplates:** The Game settings tab of the nameplate options has a Plate distance slider. It shows how far plates reach now and gives you the chat command for the distance you pick, ready to copy, since the game lets only you change this setting.

### Improved
- **Shaman:** Right-click the shield or a weapon imbue icon on the Shaman Cooldowns bar to pick which one it casts, such as Rockbiter, Flametongue or Windfury. The menu lists the ones you know and works out of combat.
- **Chat:** The chat setup keeps everything in your main chat window, also with the Whispers, Loot and Channels tabs: experience, honor, reputation, currency, tradeskills, pet and target icon lines, channels and whispers show there too. Run the chat setup again to add them.
- **Gamepad:** The Classic movement key set puts bars 1 to 3 on 1-5 R F G V X Z C, with Shift for bar 2 and Ctrl for bar 3, so T is free and V is used. The Consumable Bar keys move to Ctrl + X, Z and C. Take the set again to get the new keys.
- **Chat:** A whisper window shows the contact's name in their class color and their race and class under it, also for players outside your friends list and guild. Their level shows once the game has seen it (group, target, mouse-over, nameplates) and stays for the session.

### Fixed
- **Shaman:** Picking an Earth or Fire totem on the Shaman Totems bar sets it in Call of the Elements again. Before, the game refused it with "Only Fire Totem spells can go in that slot", because the two slots were swapped.
- **Shaman:** The tooltip of the Shaman Totems bar opens beside the bar, so it no longer covers the totem lists that open above the buttons.
- **Auras and cooldowns:** The Healthstone reminder shows only when you or a warlock in your group can make one, so a warlock who has not learned Create Healthstone yet is no longer asked for one.
- **Unit frames:** Player names in Cyrillic, Korean or Chinese show their letters on the target frame and every other unit frame instead of empty boxes, also on the game's own frames when EldoUI styles them.
- **Chat:** Whisper windows, their history and the chat message line show names and messages in Cyrillic, Korean or Chinese with their letters.
- **Windows and skins:** The friends, guild, who and group finder lists, the damage meter and the death recap show names in Cyrillic, Korean or Chinese with their letters.
- **Chat:** Shift-clicking an item, spell or quest while you type in a whisper window puts its link in the window's message line at the cursor, like the game's chat box.
- **Map and minimap:** Continent and world maps show only Transport, instance entrances and your own notes, so they are readable again. Zone and city maps show everything. Map Notes has an Also on continent maps tick for each group; City services stay on zone and city maps.
- **Windows and skins:** The side tabs in the character window show their own icons whole and at the same size, inside an even border. The Titles and Equipment Manager tabs no longer show cut-up pieces of other art.
- **Layouts and move mode:** The zone toast sits under the ready check, clear of the alerts beside it, also with Notifications off. The ready check moves up a little and the countdowns move above the spell alerts. Modern Center, Portrait Staggered and Nameplate Focus stay as they are.
- **Layouts and move mode:** On 16:10 screens, bigger action bar buttons, a larger minimap, wider unit, party and raid frames and a wider micro menu no longer push frames on top of their neighbors.
- **Layouts and move mode:** On 16:10 screens, the boss info box, the raid warning, the loot toasts and, in Close Combat and Nameplate Focus, the ping feed get their own spots where they touched a neighbor.
- **Layouts and move mode:** On 16:10 screens, Portrait Staggered's extra ability button sits a little lower and Vanilla Original's target of target a little higher, clear of their neighbors, also with bigger bar buttons.
- **Layouts and move mode:** On 16:10 screens, the Battle.net toasts stay clear of bigger action bar buttons in Close Combat, Compact HUD, Open Center and Modern Center, of wider player frames in Widescreen Edges and of wider party frames in Nameplate Focus.
- **Layouts and move mode:** On 16:10 screens, the death recap in Twin Orbs stays clear of the boss frames.
- **Layouts and move mode:** In Vanilla Original, popup dialogs open below the top notices with the Clean, Healer, Perl or Portrait unit frames, so they no longer cover the target or the target of target.
- **Layouts and move mode:** The Blizzard-like layout no longer offers the large action bar buttons: on 16:10 screens they pushed bar 4 over the game's micro menu row.
- **Info Bar:** The Gold readout counts from your first coin. With less than one gold it shows your silver and copper instead of 0, in the Gold only and short formats too.
- **Layouts and move mode:** Leaving Twin Orbs no longer leaves your health and power orbs stacked in a corner. The orbs stay with Twin Orbs and your player frame takes the new layout's own style, also when you keep your look. The layout question says so first.
- **Options:** The frame preview on the Unit frames page always fits inside its strip, shrunk with its shape kept when the frame is large, so it no longer covers the settings below it. A power bar or orb on its own position is no longer drawn under the frame in the preview.
- **Action bars:** A click on a Consumable Bar button uses its item again when the game casts on key press, and its keys work on the press. Pet feeding, fishing, raid tool, travel, bag action and quick menu buttons act on a click the same way.
- **Gamepad:** Check my keyboard in the key set window highlights the key to press without a Lua error.
- **Localization:** The Text tags tab on the Lists and tags page shows in Danish too.
- **Gamepad:** Show the changes on the spell rank prompt opens the key set window without a Lua error.
- **Gamepad:** Apply and Undo last Apply in the key set window no longer freeze the game or stop half way while the window is open.
- **Leveling and quests:** The Party Quests panel moves when you drag its title and keeps the new spot.
- **Leveling and quests:** The Party Quests panel opens in the top left, clear of the quest tracker, so the two lists no longer show through each other. Modern Center, Portrait Staggered and Nameplate Focus keep the spot they had.
- **Leveling and quests:** In the healer setup of Blizzard-like, Hunter and Sanctum, the Party Quests panel opens a little higher, so it no longer covers action bar 8.
- **Combat:** The damage meter skin no longer causes a Lua error at login while the meter still shows rows from a fight.
- **Action bars:** Picking up or placing a spell during combat no longer shows "Interface action failed because of an AddOn" when EldoUI's bars replace the game's extra bars.
- **Unit frames:** Resource bars and a detached player cast bar set above or below the cooldowns keep their spot and keep updating while the cooldowns can't be measured, and sit on their own mover when there is no cooldown row.
- **Auras and cooldowns:** The boss-mechanic aura slots next to your debuffs follow your settings again after a layout that couldn't finish, without a reload.
- **Map and minimap:** Turning the minimap off during combat keeps it off after the fight, instead of EldoUI's minimap coming back.
- **Other addons:** Turning an addon's layout spot off and on again during combat keeps your last choice after the fight, instead of sending the addon back to its own spot.
- **Chat:** Player notes, chat levels, guild mutes and Streamer Mode recognize players who have a surname, and a note saved under the surname moves to the right player.
- **Saved settings:** Put back on the Saved data page waits until you are out of combat, like Restore backup and Undo restore.
- **Bags and loot:** The bank's buy-a-tab button no longer changes during combat; it updates as soon as the fight ends.
- **Bags and loot:** The merchant's All items grid opens and refreshes again when a price or stock text has a fractional width.
- **Unit frames:** A detached player cast bar set above or below the cooldowns takes its place on the cooldown stack again, past the resource bar, the item row and the tracking bars.
- **Notifications:** The ready check, its countdown and the dungeon-ready timer show at the game's own spot with no Lua error when their EldoUI position can't be read.
- **Unit frames:** With the name above the bars, as in Blizzard-like frames, the target of target and the pet frame sit above the target's and your own name with a clear gap instead of covering it. A frame you dragged stays where you put it.
- **Unit frames:** The target of target never rises over the game's totem bar when you move that bar.
- **Group frames:** Names and health values on light class colors, such as a priest's white, a mage's light blue or a paladin's pink bar, get a thick dark outline and shadow, so they read on the bar and on its empty part, whatever your font outline setting.
- **Leveling and quests:** The quest tracker's +/- button sits on the tracker's own top row, next to its fold arrow, so it no longer covers the word "Total" on the Split Timer under the minimap.
- **Group frames:** Pet frames, and any group frames with their auras turned off, no longer set aside aura icons they never show, so they use less memory. Turning their auras on adds the icons as before.

## [0.7.1000] - 2026-11-04

### Highlights

- Twin Orbs adds an eleventh layout, with health and power orbs, a shared action-bar tray and the Infernal Stone skin.
- Gamepad Mode UI offers a controller layout, with your usual frame positions kept for switching back to mouse and keyboard.
- Undo for layout, pack and setup changes keeps the last three changes of each profile across reloads.
- Supported addons can follow your layout's reserved spots, with per-addon opt-outs and Undo.
- Loot rolls show group choices and results, and loot toasts can wait until combat ends.
- Rare Alerts adds a session history, sharing and quiet-zone controls for rare, treasure and event cards.
- The Info Bar adds session gold and XP rates, a group roll tracker and mail information across your characters.
- Encounter Timeline keeps the next-event icon with its bar and separates nearby timer icons.

### Setup and profiles

#### New

- Version 0.7.1000 starts with a fresh EldoUI profile while keeping your Journal and account progress.

#### Fixed

- Choosing the layout already in use during setup keeps your customized frame sizes and styles.
- Your latest setup changes stay available to undo after a reload or a new login.
- The import preview follows profile changes while its window is open.
- Accessibility choices that wait for combat to end stay with the profile where you picked them.
- Paused setup choices now stay intact when saved progress cannot be resumed safely.
- Profile backups preserve your previous setup when a backup cannot finish.
- Undoing setup restores the active profile correctly and preserves later profile choices.
- Shared profiles and preset packs keep imported layouts and their inherited settings together.
- Imported layouts now apply to the selected profile, with Undo restoring the previous layout.
- Imported layouts keep the positions they use on narrower screens and with larger frames.
- Revised layouts use new versions, so existing profiles keep their selected layout and dragged frames.
- Imported layouts can preserve supported frame-to-frame corner links while keeping the rest of your native setup.
- Undo for layout, pack and setup changes works after a reload or a new login: EldoUI keeps the last three changes of each profile, and each one holds only what it changed, so memory and the saved file stay small.

### Layouts and move mode

#### New

- A new layout, Twin Orbs: your health and power as two liquid orbs at the ends of the action bars, with your target centered above them and both action bar rows in one stone tray. It comes with the Infernal Stone skin and the Garnet accent.

#### Improved

- In move mode and Edit Mode, windows that open on one spot share one box with all their names; right-click picks the one to drag. A name too long for its box sits on a tab outside it, and Edit Mode's own windows stay above EldoUI's boxes.

#### Fixed

- Typing a layout's name after /eui layout now applies the same version of that layout as the layout picker.
- Cooldown placement updates with the consumable bar and returns to normal when the consumable bar is turned off.
- Layout updates safely handle unavailable private-aura settings and frame anchors.
- Resource-bar mover previews update correctly when a bar returns to the main stack.
- On 16:10 screens, wider party-frame styles stay clear of incoming combat text.
- Fanfare's glow stays within its frame, with a lower spot on narrow Portrait Staggered layouts.
- Only your selected leveling guide uses the layout's guide spot; switching guides preserves manual positions and explains when a reload is needed.
- Optional aura columns have separate positions from nearby panels in narrow-screen layouts.
- Every layout now has room for the whole bag bar with all its slots: the micro menu, the extra action button or a side bar next to it moved a little where they touched it, and the Large micro menu style is grayed out in the layouts where it doesn't fit.
- In move mode the shopping list no longer covers the boss mod info box or the target frame. In Modern Center the two boxes still share a spot, since the shopping list shows at a vendor and the boss info box in a boss fight.
- In Compact HUD the focus frame no longer touches a wide group pets grid.
- On a 16:10 screen the waypoint arrow and its coordinates sit below the talking head, and in Portrait Staggered the Battle.net toasts and the ready check get spots clear of the bars and the combat text.
- With a larger minimap or larger action bars, the durability figure, the waypoint arrow and the Battle.net toasts move aside instead of sitting under them, and the Large action bars style is grayed out where it doesn't fit.
- In Widescreen Edges the loot toasts sit beside the loot feed instead of over its newest lines.
- The death recap sits a little to the left, clear of the boss info box and the incoming combat text, and in Modern Center the boss warnings and the red error text no longer touch.
- In Blizzard Bottom Block a shaman's totem bar sits a little higher, so a taller target frame style no longer pushes the target of target onto it.
- The second info bar on its own mover takes the free stretch of the top edge instead of the whole width, clear of the minimap, the buffs, the farming bar and the mirror timers, and in Modern Center it sits under the first bar. A width you set yourself stays.
- Nameplate Focus puts its timer-bar debuffs beside your buffs, so they no longer cover the boss frames, the quest tracker or the camp panel. In Blizzard Bottom Block the totem bar clears target of target.
- Loot toast cards stack in one shared column at the right of the screen in every layout, with room for four cards at once.
- A wide micro menu style (one strip, mouse-over, minimal or large) now goes to the right edge just above the damage meter instead of over it. With large action bars, Eldo-Dark puts its bag bar there too.
- In Vanilla Original the two-row micro menu style is marked as too large, as it would cover the damage meter.
- With the large minimap style the quest timer moves down together with the quest list, so the list no longer covers it.
- In Nameplate Focus the swing timers sit a little lower, so the player cast bar of the Blizzard-like unit frames no longer touches them.

### Gamepad

#### New

- Gamepad Mode UI: when you start playing with a controller, EldoUI asks once whether to place its frames for controller play. Nothing changes until you choose, Not now asks again next session, and Don't ask again stops the question on that character.
- With Gamepad Mode UI on, your player and target frames, cast bar, resource bar and cooldowns sit in one column above the game's gamepad bar, clear of its radial menu, with the swing timers above. Your layout and dragged frames come back when you turn the gamepad interface off.
- When you turn the game's gamepad interface off, Gamepad Mode UI offers Restore now to put Edit Mode back on the layout you used before, instead of the game's Modern layout. Nothing switches until you choose, and in combat it waits for the fight to end.
- Gamepad Mode UI has its own section on the Layouts page (turn it on or off, the question, the game's Controller settings, Restore now and the controller spells), and the setup gets a Controller step when you have a controller.

#### Fixed

- The controller layout description is shorter, with a separate explanation for your controller addon.
- Reset position and Reset dragged frames in Gamepad Mode UI return inherited frame positions to the layout while keeping your mouse-and-keyboard positions for when you switch back.
- With "Positions per Edit Mode layout" on, EldoUI's frame positions for the Modern, Classic and Gamepad layouts stay with their layout when you change the game's language, and the positions you saved before carry over.

### Unit frames

#### New

- The player frame can be two orbs: your health and power as liquid orbs held in your skin's ring, with the values in the middle and liquid that swirls slowly (or stands still if you like). The new Orbs style sets it up with a long target bar to match.
- With the Infernal Stone skin, a winged demon statue kneels on a carved column beside each orb. You can turn the statues off in the Orbs options.

#### Fixed

- Turning the module off keeps unit frames hidden after combat.
- Choosing another addon's player frame also releases EldoUI's detached cast and power bars, while keeping your target, focus, group frames and saved positions.
- Cast bars keep the full spell-name space when the game reports no spell target.
- In the Classic frames style, the target of target and pet frames show the name a size smaller, so a name fits under their short bars instead of ending in "...". Every frame also has its own Name size on its Text tab.

### Group frames

#### New

- With a supported group frame addon, its group frame sits on the layout's party spot and moves to the raid spot when your group becomes a raid. Save the spot keeps it there without EldoUI too, with an Undo.

#### Fixed

- Turning the module off keeps group frames hidden after combat, even when the group changes size or you switch profiles first.
- Party and raid frames keep their rows and columns aligned when you change styles in a group.
- Saving or undoing a supported group-frame addon's position refreshes its first panel correctly.
- A saved bottom-center healer preference keeps the normal side-grid size on layouts that only support the side position.
- Long Ready Report summaries scroll inside the window and refresh without cutting off the last lines.
- Ready Report stays closed during a pull countdown when a new ready check starts; opening it manually remains available.

### Action bars

#### New

- A new option puts one panel of your skin behind bars 1 and 2, so both rows sit in a single tray.
- After a talent reset, a talent spell you had on a button of your own choosing goes back to that button when you learn it again. It follows your choice for new spells, on empty buttons only and with an Undo.
- The Key sets window has a Controller view: your class spells go on the game's controller bars in the same order as your keys, with Apply and Take back spells. Stance and form spells go on the game's stance bar of the stance or form you are in.

#### Improved

- Central proc alerts and action-button glows have separate choices when another addon provides them.
- When you import another UI's profile, the spot of its extra action button goes to the Zone Ability box, and the import preview says so in plain words.
- When you change a key binding, EldoUI's bars take the new key a moment later and set only the keys that changed.

#### Fixed

- Turning off the action bars keeps them hidden when combat ends or you switch between mouse and controller.
- Resource-bar changes update attached cooldown and consumable rows without repeatedly moving them.
- Turning off proc-alert placement restores its previous position and appearance while preserving later manual changes to the alerts and their settings.
- Choosing another addon's action-button proc glows removes EldoUI's duplicate glow while preserving your central alerts and other bar settings.
- Taking controller spells back leaves anything on your cursor untouched and asks you to put it down first. Apply and Take back confirm inside the Key sets window.
- A spell you keep on the controller bars is now also placed on its keyboard button when you apply a key set with class spells.
- With the game's gamepad interface on, the Cooldown Manager's icons no longer show keyboard keys.

### Talents and spells

#### Fixed

- The talent planner refreshes changed talent trees without requiring a talent-group switch.

### Auras and cooldowns

#### New

- Each aura group has its own visibility rules, such as only in combat, only in a group or only in one talent group, and can show only in one of your stances or forms. Every group still shows as before until you change it, and move mode always shows them.
- Each aura group can play a sound when one of its auras starts and another when it ends, also in combat. The game plays the sounds itself; both are off until you pick one.
- With a supported aura icon addon, its first six icon groups sit on the layout's aura icon spots that EldoUI's own aura groups leave empty, and follow a layout pick. Save the spot keeps a group there without EldoUI too, with an Undo.

#### Fixed

- Cooldown Pulse combines repeated spell updates and cancels pending refreshes when they are no longer needed.

### Combat

#### New

- With a supported swing timer addon, its swing bars sit on the layout's swing timer spots, and EldoUI's own swing timer steps aside while it is on. Where the addon keeps its own spot, Save the spot keeps the bars there without EldoUI too, with an Undo.

#### Improved

- The Encounter Timeline is one frame: the big icon of the next event sits at the bar's now end, both move together as one box in move mode, and an event in the big icon leaves the bar so it shows only once.
- If you moved the Encounter Timeline's big icon on its own before, it now sits with the bar again and its old place is let go. A bar you moved stays where you put it.
- Encounter Timeline icons never cover each other, even in a busy fight: close timers share two separate lanes, a timer with no room moves on a little and shows its seconds, waiting events each get their own spot, and the tick numbers sit under the bar instead of between the icons.

#### Fixed

- Turning your own swing bars off and back on no longer leaves an expired swing frozen on screen.
- When you show EldoUI's battleground bars next to your boss mod's own battleground timers, they move to the boss frames' spot, so they no longer sit under the boss mod's timer bars, in every layout.
- After the Combat only style of the combat HUD, picking another combat HUD style shows the damage meter out of combat again.

### Info Bar

#### New

- With a supported data bar addon, its bottom bar takes the layout's data bar edge. When its bar sits on the top edge, Save the spot moves it to the bottom, with an Undo.
- Three new Info Bar blocks, Gold per hour, XP per hour and Time to level, share one session that goes on over a reload. Their tooltips show what you earned and spent, your best hour and your rested XP, and a right-click starts a new session.
- A new Rolls block on the Info Bar keeps track of /roll in your group: its window lists each roll highest first and marks the winner, a tie, a second roll and a roll outside the usual range, with buttons to roll, to pass and, for the leader, to announce the winner.

#### Improved

- Info Bar blocks no longer run into each other on a narrow bar: the blocks nearest the middle step aside behind a » button, whose tooltip shows them and whose menu still opens them, and they come back once there is room.
- The Info Bar's Mail block now covers all your characters: its tooltip lists each one with mail waiting and the time until its first letter runs out, the block turns yellow, then red, before a letter runs out, and a chat line at log-in says which characters to visit.

#### Fixed

- The Info Bar's coordinates and item level blocks show their full names in the options and in the » tooltip, in Danish too.

### Chat

#### Fixed

- The errors tab shows the indented lines of an error's details as plain spaces.
- In the chat list editors, the feedback line ends before the buttons at the bottom of the window.
- A group, guild or message window post made while the game doesn't allow chat messages now says so, is no longer marked as posted, and can be sent again; a refused typed line stays in its box.
- The errors tab in the chat window opens again when the error log holds an older entry without a type, and lists that entry as an error.

### Bags and loot

#### New

- With a supported loot addon, its roll bars and loot feed sit on the layout's loot spots, and its loot window too while it does not follow the cursor. Save the spot writes them into the addon's own settings, with an Undo.
- With a supported bag addon, the bag and bank windows open in the layout's bag and bank corners at a size that fits them. Where the addon keeps its own spot, Save the spot keeps them there without EldoUI too, with an Undo.
- EldoUI's roll bars show how many in your group picked Need, Transmog, Greed or Pass so far; point at the counts for the names and who has not chosen yet.
- Loot toasts show four cards at once by default (Toasts at once), and more loot waits its turn instead of piling up. A card stays while the mouse is over it, an optional sound plays once per burst (with its own pick for legendary items), and legendary items read "Legendary!".
- Loot toast cards for what you loot in a fight wait and show, in order, when the fight ends, so they stay off your combat screen. The loot feed still lists loot as it drops.
- The loot feed and toasts can show what group members loot (with its own lowest quality and time on screen), experience added up in one row, and honor, each with its own switch.
- Loot feed rows mark a currency at its cap and can show the item's total in your bags; items you make have their own switch, and a right-click closes a row.
- EldoUI's roll bars stay after you roll: the bar shows your choice, then who won with their roll, or Everyone passed. Each bar also shows the item level, a green border for an upgrade and a red timer when time runs short.
- EldoUI's loot window has a Link button: one click posts the items' links to your group, raid or instance chat (or Say), highest quality first, from the quality you pick. Long loot lists stay within the chat's line length.
- EldoUI's loot window can mark each item: BoP, BoE or BoU on the icon, the upgrade arrow, New look for an appearance you have not collected and Starts a quest, plus a slot and type line and the stack's vendor price if you want them. Each mark has its own switch.
- Make your own bag categories, each with a name, color, search and priority, and order every section of the Categories view. Drop an item on a section title to file it there, or share your categories with a string. Old category searches carry over.
- Group stacks, on the Categories tab, shows the stacks of one item as one slot with the total count in the Categories view, and every stack apart again while a vendor, the mailbox, the bank or a trade is open.
- A Searches button on the bag and bank windows keeps your favorite searches for one-click use, and its Search help lists every search word with an example you can click to try.
- New slot marks: a red icon on items your character can't use yet, a mark on equipment set items, a fade on what an open vendor, mailbox, auction house or socket window can't take, and Alt-click on an item flashes every slot that holds it.
- At the bank, the bank window sells the next bank tab from a plus on its bag bar, with the game's own confirm and the cost in the tooltip. A Deposit button puts everything that fits into the bank, and right-clicking a bank tab renames it or picks the items it takes.
- The guild bank can open in EldoUI's own window (Bags page, Guild bank: EldoUI window), with tabs, search, the item and gold logs, tab info and the game's own gold and tab dialogs. Every click works as in the game's window.

#### Fixed

- Help waits for the current opening, so closing and reopening the window does not show it early.
- The merchant grid keeps item names, complete prices and stock counts in separate space when text grows.
- Item comparison details stay below their action buttons when text size or the window changes.
- Confirming a merchant purchase safely stops if the item's details disappear before you accept.
- A short bag section keeps the lines on both sides of its name clear of the fold arrow.
- The bag and bank window titles sit on the same line as the character button and the close button.
- Long loot-roll lists scroll within the screen, keeping every item and manual choice reachable without changing your saved position.
- Turning off appearance markers now frees their cached item data.
- Supported bag windows keep their layout spot when bank contents finish loading, without changing saved positions.
- The shared bank and its pages are named Account bank throughout the bag and bank windows.
- A temporarily missing vendor item no longer interrupts restocking or a purchase question.
- The loot roll bar shows the item name above the "binds when picked up" line, and the Loot Guide box beside a roll shows its two lines one above the other.
- On EldoUI's roll bars, the Binds when picked up line no longer covers the item's name.
- Master looting works with EldoUI's loot window: clicking an item opens a give menu with everyone who can take it, by class in a raid, your Banker and Disenchanter first, soft reserves after the names, and Request roll. Epic items ask before they are given.
- In the bag window's Categories view, an item you sold or moved no longer leaves its picture behind on the window.

### Journal

#### Fixed

- A damaged backup no longer clears your choice to keep a restored journal unchanged.
- Twin Orbs now applies its matching Book look when the journal follows the layout.
- Imported companions keep hyphenated last names, and older spellings merge their history without losing time or quest partners.
- Dungeon route sharing clearly says when the game is holding addon messages back.
- Chapter statistics in the Book keep their full text on narrow pages and flow onto more pages when needed.
- The Loot Guide's dungeon list is complete the first time you open it in a session, also when the loot data loads as the window opens.
- In the Database tables the name column takes the room the other columns leave, so most names show in full, and the last columns and their titles no longer run past the table's edge into the detail pane.
- The Loot Guide's PvP rewards list always shows its rewards, or a line that says why, instead of an empty column, and it builds only the rewards you scroll to, so typing in its search box stays smooth.
- The guide list, the page header line, the "Kept since" line, the character panel on For you and the welcome card's intro sit at the top of their place instead of drifting to the middle.

### Leveling and quests

#### Fixed

- Eldostar restarts a guide's search loop correctly when you switch guides or reset its progress.
- Eldostar keeps accented letters and symbols intact when shortening guide text.
- Eldostar shows a long guide title in full in its header: the title gets a slightly smaller font before it would be cut short.

### Map and minimap

#### New

- /way list opens a new Waypoints window with every waypoint by zone, nearest first: click one to point the arrow there, right-click to remove it, or export them all as /way lines to paste later. /way print still lists them in chat.
- With a supported minimap button addon, its button sits in the corner of the minimap where EldoUI's own button bin would be.
- With a supported waypoint addon, its arrow sits on the layout's arrow spot at a size that fits it. Save the spot keeps it there without EldoUI too, with an Undo.
- The addon button bin can sit on its own mover anywhere on the screen, fill in any of eight directions, gather an addon button you add by its name, and keep the click drawer open across a reload when you pick Remember the drawer.
- EldoUI has its own minimap button. It leads the addon button bin, or sits on the map's edge where you drag it while the bin is off; a click opens Move frames and a right-click keybind mode.

#### Improved

- The addon button drawer is now the minimap's own default in every layout, so Reset to defaults on the Minimap page gathers the addon buttons too. A profile that keeps them on the map keeps them there.

#### Fixed

- Waypoint titles follow the next guide goal at the same place, and renamed destinations update the arrow and stay renamed after a reload.
- Battlefield maps and widgets return to their original size when you turn off their placement.

### Windows and skins

#### New

- A new skin, Infernal Stone: charred basalt, rusted iron bands, pointed iron corner brackets and blood-red gems, with window titles in a gothic letter. It brings the new Garnet accent, which you can also pick on its own.

#### Improved

- Buttons and check boxes have a clear edge in every art style. EldoUI's windows (options, setup, Journal) are always solid, so a window opened over another no longer shows it through. Panel opacity now sets the panels on the screen, such as chat and meters.
- With the game's gamepad interface on, EldoUI's buttons in the mail, merchant, auction house and character windows step aside, so the controller cursor moves only over the game's own buttons. They come back when you switch to mouse and keyboard.

#### Fixed

- The Legacy planner places its pages before drawing their rows.
- Unavailable window artwork falls back to the game's standard look.
- Saved death recap positions and sizes work together correctly without overwriting later changes from other window controls.
- In the drawn skins, such as Vanilla Original, a frame's border no longer stretches into a striped strip past its edge after the frame changes size, as it could behind the side bars until a reload.
- In move mode's Combat view, an open mail, trade, auction house or merchant window no longer shows a box that then disappears when you hide and show the boxes. Its box shows in All frames, like every other window, and a window you don't let EldoUI move has no box in any view.
- EldoUI's questions grow to fit their buttons, so a long button label no longer runs past the window's edge with large text or in Danish.
- Rows, notes and labels in EldoUI's windows keep their own line: the Loot Guide, the installer, the options, dungeon routes, the trainer and the trade window no longer squeeze a line to nothing, draw it in the middle of a taller box or stretch a button across the window.

### Notifications

#### New

- Rare Alerts can give your gamepad a short pulse for each alert, and a longer one for a rare with a mount, pet or toy you don't own yet. It is off by default and never pulses for a quiet sighting.
- Shift-click on a Rare Alerts card opens the chat box on your group's channel (or the one you pick) with the name, the place and a map pin link. You press Enter to send it.
- A Rare Alerts card says Already done when the game tells that your character already killed or looted that rare or treasure, and Keep rares you already did quiet leaves such cards out.
- A new Rare History window lists this session's rares, treasures and events beside the rare cards: click a line for a waypoint, Shift-click to share it, right-click to remove it. It is off by default and hides in combat.
- Rare Alerts can stay quiet in zones you pick and for whole kinds (rares, rare elites, world bosses, treasures, events): a quiet sighting shows its card without sound, or nothing at all. A name you watch for is never quiet because of its kind. Pick zones on the Quiet tab.
- Rare Alerts also tells you when the game marks a treasure, a chest or an event on the minimap: a card in its own look with its own sound, and a click on it sets a waypoint. Treasures and events each have their own switch.
- With a supported rare addon, its rare popups or its rare button sit on the layout's rare card at a size that fits it. Save the spot keeps them there without EldoUI too, with an Undo.

#### Improved

- The Rare Scanner is now called Rare Alerts. Your settings, ignored rares and quiet zones stay as they are.

#### Fixed

- Zone notices leave room for compact ready checks and queue popups while keeping your saved positions.
- Ready-check button labels return to their original positions when you switch profiles or turn notifications off.
- Ready-check countdowns stop when you close the dialog or turn notifications off.
- Zone toasts keep their text spacing when Large text is enabled.
- The help-tip setting stays hidden on clients that do not support it.
- Ping feed rows keep their spacing with Large text, and narrow layouts leave room for conversations and group tools.
- Alert toasts show their title, main text and small bottom line on three separate lines again, instead of drawing the title and the bottom line over the main text.

### Other addons

#### New

- Your layout gives the frames of other addons a spot of their own at a size that fits it, and moves them along when you pick another layout, out of combat. Each addon can stay where its own settings put it, from the Other addons page or with /eui addons fit.

#### Fixed

- Choosing another resource display hides only the matching mana, rage or energy bars. Other resources remain available, and a druid's mana strip keeps a place when its main bar steps aside.
- Choosing another combo-point display hides only EldoUI's combo rows and nameplate points, leaving your other resources and saved positions in place.
- Choosing another five-second timer hides only EldoUI's spark, leaving your power bar, other resources and saved settings in place.
- Choosing another addon for the threat meter hides only EldoUI's threat display and keeps it hidden through pending updates, leaving your other combat displays and saved settings in place.
- The Other addons page recognizes more minimap, window skin, chat and healing-frame addons, while manual profile importers can run alongside your saved setups.
- A second damage meter window now lines up with the right edge of the first one, so a wider second window stays on screen.

### Options

#### Improved

- On a module's Presets tab and on the Style presets page, the style you applied last is marked, so you can see which one is in use.

#### Fixed

- The move-frame menu shows the correct Options label.
- Long sound choices use the available space, settings buttons grow with their labels, and cooldown rows use clear position names.

### Performance

#### Improved

- Action bars use less temporary memory when their layout refreshes.

#### Fixed

- Trying layouts and style presets one after another no longer makes EldoUI's memory grow until you reload: the buff, debuff and weapon enchant rows reuse their frames.
- Selling, buying or stacking items with the bag window open redraws only the bag that changed, so selling junk at a vendor no longer stutters.
- With the Loot Guide's Best in Slot page open, putting on a new item only scores the items again instead of going through the whole item list, so changing gear no longer causes a lag spike.
- Closing the auction house late in a full scan no longer freezes the game for a moment, and the prices read so far are still saved.
- The Loot Guide's gear simulator keeps to the time per frame you pick for it, Turbo included, instead of running a little past it.

### Saved settings

#### Fixed

- After going back to an older EldoUI, the settings a newer version saved are written back exactly as they were when you log out, so the newer version finds them unchanged.

### Localization

#### New

- With EldoUI in Danish, item tooltips can show a small box with the Danish word for what the item is, such as Le on a scythe, while the English name stays as it is. It is off until you tick Danish word help on the Tooltip page.

#### Improved

- The spell switches on the Buff and Consumable Reminders and Shaman Totems pages show each spell's name the way your game client writes it, in every game language.

#### Fixed

- Names and messages in Cyrillic, Korean and Chinese keep their letters on unit frames, group frames, the threat list and the other name texts, and in the chat, the message windows and chat bubbles, as they already did on nameplates.
- On a game client in another language, the Loot Guide's item lists follow the game's newest item name even after a long browse, without a reload.
- With EldoUI in Danish, the Combat Text setting that counts joined lines shows its "×3" example correctly instead of a broken letter.
- With EldoUI in Danish, the Appearance line on item tooltips says in Danish whether you have collected the look, instead of in English.

### General

#### New

- A Thanks page names the people who helped build EldoUI with code, research and testing, and the people who stand behind it. Open it from the Thanks link at the foot of the options sidebar or with /eui thanks.

#### Fixed

- Command help and text tag descriptions show choice separators as readable text.
- The chat color preview shows each sample line on its own row again, and the move mode sample titles, the trainer's "to learn now" line, the soft-reserve line on loot rolls and the boss mod status text stay at their edge.

### Classes

#### New

- **Hunter:** The Journal's Database marks the beasts you can tame with a paw and their pet family, and its Mobs table can show only tameable beasts, or one family, together with the level and place filters.

#### Fixed

- **Shaman:** The Tremor Totem hint safely stays off when loss-of-control information is unreadable.

## [0.7.0003] - 2026-10-28

### Highlights

- Your key set now belongs to your profile and knows US, UK, Nordic, German and French keyboards, and new spells land on their own key on bars 1 to 3.
- Tour helps explain new parts of EldoUI the first time you meet them, and a new character on an account you already set up gets one short page instead of the whole setup.
- Eldostar, EldoUI's own leveling guide, brings over 200 community guides for WoW: Forever in a window on your layout, with a waypoint to the next goal.
- My Adventure has a Guides page where you start, follow and search the leveling guides.
- The Journal can group a boss's loot by kind and shows a branching dungeon quest chain as a flowchart.
- On a 16:10 screen the layouts give the boss frames, the boss mod windows, the party pets and many more frames a spot of their own.
- The UI scale choice shows which scales the layouts are made for, with Auto recommended.
- Switching style presets keeps your layout tidy, and a damaged saved settings file no longer stops EldoUI from loading.

### Setup and profiles

#### New

- A new character on an account you already set up gets one short page instead of the whole setup: it uses one of your profiles as it is, with its own chat tabs, game settings, click-casting and class spells.
- The alt page lists your class's profile first, can copy a profile set up for another role, and Undo puts everything back. Open it any time with /eui attach or from the Profiles page.
- A layout whose bars show on mouse-over says so once, with a button to show them all the time, and after the setup a short help shows where to change your UI later.
- The setup's Convenience step lists every helper that acts for you, from repairs to the quest helpers, and "Recommended for me" ticks the ones that suit your class and level. The same list is the new Conveniences page under Modules.
- The Keys and spells step asks how you play: a key set or "I manage my own keys", what happens with spells you learn later and on your other characters, and whether bars 1 to 3 show their keys. Each pack fills in its answers, and nothing changes until you press Apply.

#### Improved

- The Classic and Vanilla packs start the Keys and spells step on the Number row keys, the way the game sets bar 1.

#### Fixed

- In the setup's UI scale step, a scale card with a long description no longer runs into the screen line above it or the custom scale below it, also with large text.
- An interrupted first setup resumes unfinished changes, and a setup waiting for combat to end uses your latest layout choice.
- Finishing or skipping the first setup during combat now gives you your layout as soon as combat ends.
- EllesmereUI imports keep your chosen EldoUI layout's settings and responsive placement for frames the imported layout does not move.
- A new character that starts on its class's profile keeps that profile when you run the full setup, instead of being moved to the shared EldoUI profile.

### Layouts and move mode

#### New

- When a layout keeps an action bar out of sight, a tour help draws the bar where it sits and tells you its keys still work, naming the long cooldowns on it. Keep it hidden keeps it out of sight on mouse-over too.

#### Improved

- The Vanilla Original layout now offers the Large action bar style too; your bags open on top of the bars.
- Switching between style presets keeps your layout tidy: going back to a style puts every frame back exactly as that style placed it, and a style no longer keeps settings left over from the one picked before it.
- The Blizzard-like group frames can now be picked in the Portrait Staggered and Nameplate Focus layouts, and the Healer group frames in Nameplate Focus.
- On a 16:10 screen the boss frames, boss mod windows, party pets and targets, vehicle seat, pet and bag bars, Battle.net toasts, red error text and combat text get spots of their own, clear of the chat, the bars and the damage meter.
- Style presets and the setup now say what a style does to your layout: a style that makes a frame bigger moves its neighbors to make room, and one that doesn't fit is grayed out.
- In the EldoUI Center and Nameplate Focus layouts the experience bar is now as long as action bar 1, so it no longer reaches past the side bars when they are empty or hidden. A bar length you picked yourself stays as it is.
- In move mode with test frames, an empty action bar, buff or debuff row, quest tracker, cooldown row or swing timer shows a sample in your own sizes, colors and text, starting on the side it grows from, so you see the frame the way it will look.

#### Fixed

- In Edit Mode, the EldoUI side panel stays on screen when the list of what EldoUI places is open and long; the list scrolls instead.
- The durability figure moves aside with your buffs and debuffs when the minimap is larger or round, and on 16:10 screens, instead of sitting on top of them.

### Unit frames

#### Fixed

- 3D portraits stay inside the round portrait of the original frames and the portrait rings, with the face framed a little wider, and no dark square or box shows around the portrait or beside the target any more.
- The original frame art keeps its true shape on the Classic frames style, so its portrait ring sits exactly on the portrait, also on the target of target and the pet.
- Names stay inside their name bar or health bar in every unit frame style, and Classic frames show the level by the portrait instead of above the frame, where it could cover the target of target. A level badge on your own frame always shows your level.
- With the original frame art, the small circle under the player and target portraits shows the level, as on the classic frames: the rest icon while you rest, the attack icon in combat, and on the target a skull for a corpse or a level too high to tell.

### Group frames

#### New

- With the Healer role, the Role page can put your group frames at the bottom center, above your bars: the party as one row and a raid of up to ten as two rows. A larger raid moves beside the center on its own.

#### Fixed

- In the Close Combat layout with the Healer role, the party frames no longer touch the top of your player frame.
- The group pets and the main tanks no longer sit on top of each other next to a tall raid: the one you have turned on keeps the spot and the other goes beside it.

### Action bars

#### New

- New spells land on their key: a spell you learn has its own button on bars 1 to 3, the same on every character of your class. EldoUI offers to put it there, or does it for you when you pick Automatically, on empty buttons only and with an Undo.
- Upgrade spell ranks automatically, an option you turn on yourself: new ranks move onto bars 1 to 3 and the gamepad bars out of combat, with a chat line and an Undo. Macros, spells on your keep list and buttons kept at a low rank never change.
- Fill bars 4 and 5, an option you turn on yourself: out-of-combat spells such as teleports, tracking, poisons and pet care go on the empty buttons of bars 4 and 5. Your own buttons stay, a spell you learn later joins them, and Undo takes them off.
- Two new key sets: Side-button mouse puts bar 1 on a mouse with 12 side buttons, and Shifted hand rests your hand one key to the right for more keys around it.
- The key sets know US, UK, Nordic, German and French keyboards and use the keys in the same places on each. Check my keyboard finds yours from three key presses.
- A game shortcut a key set takes gets the same new key in every set, such as Alt-R for reply, and the game keys list (`/eui keys`) shows where bags, map and the rest are. Bar 3's last three keys use the Consumable Bar: potion, healthstone, and mana potion or bandage.
- A new visibility rule, "Mouse over, out of combat", hides a bar in combat and shows it when you point at it outside a fight. Each bar from 3 up has a Show on screen switch that hides it this way, keys still working; turn off Show on mouse over to keep it out of sight altogether.
- Your key set belongs to your profile now, so it stays the same on every layout, pack and style preset. Your other characters on the profile get one offer to use the same keys, or get them by themselves when you choose Automatic, and keys you set yourself are never written over.
- After a role change, EldoUI offers to put the class spells of your new role on your bars, only on empty buttons and on buttons where it placed a spell of your old role, with Undo.

#### Improved

- Bar 3 now shows nine buttons, in a shorter row or a 3x3 block, and keeps the actions and your own keys on its last three. Widescreen Edges and Open Center keep all twelve, so bars 2 and 3 stay an even pair beside bar 1.
- The offer to move your buttons to a new spell rank is now on for everyone and also checks once at login. It only asks, and nothing changes until you apply. It steps aside while another addon moves your spell ranks.
- The spell rank check also covers the gamepad bars and finds a lower rank even where the game does not mark it, and it never suggests a rank you have not learned.
- The Cooldown Manager's Key text shows the key on every icon, only for spells on buttons you can't see, or not at all. The default is only hidden buttons: a bar you turned off or shortened, or one shown only on mouse over or out of combat.
- Every spell of every class and role now has one fixed button in the key layout. The spells you press in a fight are on the easy keys of your first two bars, and bar 3 holds what you use between pulls, such as buffs, resurrection and travel spells.
- When a bar pages on Shift or Ctrl, or your text style hides the keys on bars 1 to 3, EldoUI tells you after you apply a key set and fixes it in one click.

#### Fixed

- The keys of a bar that a layout hides keep working, also past a shortened bar's end. The hidden bar shows when you point at it out of combat, in a small box next to your bags (bars 4 to 8 at the right edge); a bar a layout switched off before comes back this way.

### Talents and spells

#### New

- A macro that names a lower spell rank, such as Frostbolt(Rank 3) after you learn Rank 4, is marked in the macro editor and the rank check. One click on Update to Rank 4 changes only the rank number, out of combat, and Undo puts it back.

### Chat

#### Fixed

- While you type in the main chat window with the input box over the tabs, a chat window you dragged out of the dock keeps its tab name, whisper icon and flash.

### Journal

#### New

- My Adventure has a Guides page where you start a leveling guide for your character, see the one you are on and the one up next, and search every guide. At the level cap, Eldostar shows nothing until you start a guide there.
- A boss's loot can be grouped by kind: quest items, weapons, armor, accessories and everything else, each with the most likely drop first. The Journal remembers whether you sort by chance or by kind.
- A dungeon quest chain that splits into several paths shows as a flowchart in the quest details: every quest is a box with your progress, joined by lines to the quests that follow it. Switch to the step list at any time, and the Journal keeps your choice.

#### Improved

- The Journal's tours follow the Tour helps switch, and Show tour helps again on the General options page brings them back too.

#### Fixed

- Opening an attunement or a class quest from a link, a waypoint or a slash command scrolls the Attunements list to it, so its row is always in view.

### Leveling and quests

#### New

- Eldostar is EldoUI's own leveling guide: over 200 community guides for WoW: Forever, step by step in a window on your layout's guide spot. Goals tick from your quest log, bags, level, reputation and professions, and a waypoint points to the next goal.
- The setup's Other addons step and Eldostar's options let you pick the one leveling guide that takes the guide spot: Automatic, Eldostar, RestedXP or Off. EldoUI never turns the other guide addon off.

### Map and minimap

#### Improved

- The minimap styles say when they can't show yet: while the game's own minimap is in use, Style presets and the setup tell you how to turn on EldoUI's minimap.
- With a larger minimap style, the buff and debuff rows move out with the map and keep their distance to it, and on a round map the Split Timer and the quest list keep clear of the map's ring.

### Notifications

#### Fixed

- On a Hardcore character with the card title color set to Plain, as in the Quiet style, death and PvP cards show their title in plain white instead of the accent color.

### Other addons

#### Improved

- EldoUI recognizes many more addons that do one of its jobs. Nameplate, buff, loot window, tooltip, chat, waypoint and world map addons now make EldoUI's own version stand back, so the two never draw the same thing twice, and you pick who handles each job on the Other addons page.

### Options

#### New

- The Other addons page has a new list, Also done by EldoUI: addons that run fine next to EldoUI but do a job EldoUI already does, in full or in part. For an addon whose whole job EldoUI does, one click turns it off for this character.

#### Fixed

- Every line of a wrapped dialog checkbox label can be clicked without covering the buttons below it.
- Long page names in the options list and long page descriptions wrap onto a second line instead of being cut off, and a few choices with long names have shorter ones, in English and Danish.

### Performance

#### Fixed

- The rare scanner reads the rare markers once for each burst of map updates instead of on every single update.

### Saved settings

#### Fixed

- EldoUI loads even when part of its saved settings file is damaged: a broken profile list or profile starts over as a new profile, and the damaged part is kept aside instead of being deleted.
- Import refuses a string that unpacks to more than the import size limit or carries damaged frame positions, with a clear message, before it changes any setting.

### General

#### New

- Tour helps explain something new the first time you meet it: move mode, the Layouts and Blizzard UI pages, your keys after you apply a key set and the chat tabs the setup made. Each one shows once, and the Tour helps switch on the General options page turns them all off.
- More parts explain themselves once with a tour help: the bag window, the vendor list, Open all in the mailbox, the auction house tabs, healer click-casting, fishing mode, the minimap button rail, styles, keybind mode, profile rules, the guide window and Edit Mode.

#### Improved

- The UI scale choice in the options and in the setup shows which scales the layouts are made for: Auto is recommended, and every other value is marked as supported or not recommended, with a short reason.

#### Fixed

- The update note's title, buttons and checkbox follow your selected language when you open it again.
- EldoUI keeps recognizing WoW: Forever if the game renames its client type at launch, so your characters' saved data and your look stay as they are.
- /eui commands still work when you type a period, comma or other punctuation right after them, such as /eui errors.

### Classes

#### Fixed

- **Paladin:** Training lists Righteous Fury at level 10 and Retribution Aura at its current trainer cost.
- **Shaman:** Training shows the current trainer costs and the level 50 rank for talented shamans, so the rank after it can show as well.

## [0.7.0002] - 2026-10-23

### Setup and profiles

#### Fixed

- The Modern pack shows keybinds and macro names on the action buttons.
- The setup's first click shows your layout's action bars right away, instead of a half-finished screen until you finish the setup.

### Layouts and move mode

#### Fixed

- Vanilla Original's two right-edge columns and Modern Center's right-edge column hide their empty buttons, and Vanilla Original suggests Class Power pips without a second power bar, since its player frame already shows your power.
- In move mode, the arrow keys nudge the selected frame, as its tip says: 1 unit, or 10 with Shift.
- In Modern Center, the cooldown Buff Bars sit clear of the pet and pet target frames.
- Nameplate Focus turns the target of target frame off along with the target frame, so no lone frame is left on screen; another layout brings both back.
- In EldoUI Center and Modern Center, the bag bar, the micro menu and the zone ability button stack in one column at the bottom right, clear of a damage meter docked in the corner.
- EldoUI Center's second and third action bars hide their empty slots, so a new character's first screen no longer shows rows of empty boxes.

### Unit frames

#### Fixed

- With the Classic frames style, the player and target portraits show the face at its true shape inside the Vanilla ring and the original portrait circle, and a new style or look updates the picture at once.
- On Boxed unit frames, the race and class text and the name keep clear of the class badge and the PvP and elite marks on the frame's corner.
- An extra resource bar that shows its value as a percent no longer raises an error while the game keeps your power values hidden.

### Group frames

#### Fixed

- With the raid manager side panel skinned, the ready check, role poll, countdown and option buttons show their icons again.

### Action bars

#### Fixed

- In Vanilla Original, the vehicle exit and zone ability buttons sit clear of the gryphons. The setup grays out the Large action bar style for this layout, since its bigger gryphons leave no room beside the bags.
- Blizzard Bottom Block's two side grids hide their empty buttons, and show them while you drag a spell.

### Info Bar

#### Fixed

- The Info Bar's Two bars style keeps zone, coordinates, experience and reputation on its second bar, so nothing overlaps when that bar sits in the chat window.
- The Info Bar's memory block and its tooltip show the same total, and the open tooltip no longer adds work every few seconds.

### Chat

#### Fixed

- While you type in the chat box over the tabs, the tab names, whisper icons and new-message flashes no longer show through it.

### Bags and loot

#### Fixed

- The auction house tabs EldoUI adds are named Shopping List, Quick Sell and Cancel Undercut, so they no longer read like copies of Blizzard's Buy, Sell and Auctions tabs, and they stay inside the window with large text.

### Journal

#### Improved

- The printable journal page uses the book fonts on your computer and no longer asks a web font site for its fonts when you open it.
- The copy box of a journal or runs backup code names the button to paste it into once, and the run count's tip says plainly that the Instances module records the runs.

#### Fixed

- The Loot Guide's PvP rewards list says why it is empty: the filters, with a button to clear them, or the loot data still loading, switched off or not installed. When the data arrives, every reward shows at once.
- The guild attunement list's "Seen" column is named "Sent", since it shows how long ago each member sent their data.
- The Loot Guide's dungeon list keeps the wing names of Dire Maul, Blackrock Spire, Scarlet Monastery and Stratholme, and the wishlist alert names the wing you entered.
- Looting and moving items no longer makes the game hitch while the journal is open, and accepting or finishing quests no longer reworks the where-next list each time.

### Map and minimap

#### Fixed

- Buttons on the minimap's side rail keep the rail's order, whichever one you put there first.
- With the Large minimap style, the Split Timer and the quest list move down with the bigger map instead of sitting under it, in every current layout.
- On the world map, boat, zeppelin, Deeprun Tram and portal pins show a ship, an airship, a tram car and a swirl in their own colors, instead of plain colored blocks.
- With the minimap buttons skinned, the calendar button shows its calendar icon again.

### Windows and skins

#### Fixed

- With the Modern (flat) look, every EldoUI window has an edge you can see against the world, and the options window steps aside while the setup is open and comes back after it.
- The EldoUI button in the game menu is there from a new character's first login, before the setup is finished.

### Options

#### Improved

- The Version check option says that it sends your version as a hidden addon message to guild and group members who run EldoUI, never in chat.

#### Fixed

- Picking another style brings back the bars and buttons an earlier style hid or faded, such as the XP bar after Mouse-over only or the right chat panel after Split.

### Localization

#### Fixed

- In Danish, the Alts window's last-online column reads "Sidst set", the Journal's next trip reads "for level", and Reset size, the Macro Editor's subtitle and the Loot Guide's Dungeons caption are no longer cut off.
- With EldoUI in Danish, the options page subtitles, the Glows and Screen area tabs, the Safety page, the Blizzard UI switch notes, the search boxes, the Journal's place phrases and every date read Danish, with the day first.

### General

#### Improved

- The install guide and the release notes name the WoW: Forever game folder, _forever_; the guide tells beta players to install EldoUI there again.
- The note after an update has a "Never show again, even after updates" tick box; the switch on the What's new page turns the note back on.

#### Fixed

- The bug report form and the support pages name the error window's Report button, as the game shows it.
- After the micro menu's Mouse-over style, any other style shows the micro menu and the bag bar again, and the Mouse-over style's description says so.

## [0.7.0001] - 2026-10-21

### General

#### Fixed

- Every EldoUI version can be downloaded as a zip from its release page.

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

### Setup and profiles

#### New

- Four roles in the setup and on the Role page: Melee, Ranged, Healer and Tank. Ranged also shows the five-second rule on your mana bar.
- Every layout or pack change can be undone: press Undo on the alert after the change, or type /eui layout undo. Settings you changed yourself since stay as you set them.
- A new Keys and spells step, also on Express, shows your key preset, class spells, macros and rank upgrades before anything changes. Your bars change only when you press Apply, your own actions, macros, items and kept ranks stay, and one Undo puts it all back.

#### Improved

- Saved profiles and dragged positions carry over after the update, with a copy of your screen kept under your own layouts.
- A profile that used the older Damage role moves to your class's Melee or Ranged role by itself, and every frame stays where it was.
- The setup waits while the game asks whether to skip the intro cinematic, and while Details! or Questie show their own first-start windows, and opens once you have answered.

#### Fixed

- A profile that names a layout that is not installed now says so once and keeps your saved layout choice.
- A pack applied from the Overview or a pack string now also sets its role, and choosing the Healer pack after another pack no longer leaves raid frames covering your own frame.

### Layouts and move mode

#### New

- Ten built-in layouts, each with its own shape on screen: Vanilla Original, EldoUI Center, Modern Center, Blizzard Bottom Block, Portrait Staggered, Compact HUD, Widescreen Edges, Close Combat, Open Center and Nameplate Focus.
- EldoUI Center is the new default for new profiles: player and target sit level with the cooldown row, and the action bars form one block at the bottom with a narrow wing on each side. Profiles from earlier versions keep the layout they used.
- In move mode, the pet and stance bars can be laid out Horizontal, Vertical or as a Grid, and the action bars, pet and stance bars, micro menu and bag bar have Size and Spacing menus.
- Move mode's frames menu has Find a frame: pick any frame to show, select and flash its box, and bring a frame that ended up off the screen back to the nearest edge.

#### Improved

- Picking a layout gives the same result from the Layouts page, /eui layout, the Overview, a pack and the setup: the layout's skin, Blizzard windows and suggested styles, nameplates included.
- Frames you dragged stay where you put them when you change layouts, unless you tick "Put frames I dragged back in the layout's spots". Applying the layout and look you already use changes nothing.
- If you picked a skin yourself, choosing a layout asks once whether to use the layout's look; "Keep my look" is the default.
- The Layouts page, the Overview and the move panel share one picker for built-in and saved layouts. The Overview and move mode show your layout, role, skin and Blizzard windows.

#### Fixed

- A micro menu or bag bar you moved in an older version stays where you put it, and the bar and macro check boxes on the class setup page remember your choice.

### Unit frames

#### New

- A new Classic frames style gives the player, target, target of target and pet frames the shape of the original frames, with a round portrait.
- With the Vanilla Original skin, frames sized like the originals wear the game's own classic frame art, with the elite and rare dragons on the target. The Vanilla Original layout shows them as soon as you pick it.

#### Improved

- A unit frame graphics choice that does not fit your layout is grayed out, with the reason in its tooltip.
- The unit and party frame style with the boxed 3D portrait and name bar is now called Boxed.

#### Fixed

- Cast bars no longer show an error when an enemy casts something whose details the game keeps hidden, and keep the EldoUI look.
- Turning Unit Frames off brings Blizzard's own unit frames back at once, without a reload, unless they were set to be replaced.

### Group frames

#### Improved

- Party and raid frames keep the empty part of the health bar dark and clearly apart from the frame art in every skin, and the Minimal party style shows a slim mana bar on healers.

#### Fixed

- With the Healer role, raids that use the Mid or Large raid settings keep the larger healer frames too.

### Nameplates

#### Improved

- Nameplates do much less work in big groups and cities: each plate listens only to its own unit, cast bars and hover update only while there is something to show, and quest progress and NPC titles are read once per change.
- EldoUI's nameplates wear your skin's frame edge, the same thin edge as small unit frames, and follow your unit frame graphics choice. Target, focus and style rule border colors still come first.

#### Fixed

- Turning off EldoUI's plate size after changing Blizzard's nameplate scale gives back the size the game uses now.

### Action bars

#### New

- With the Vanilla Original skin, a one-row bar 1 sits on the classic stone tray with a gryphon at each end, the stance bar gets its classic stone, and the micro menu and bag slots wear their classic buttons.

#### Improved

- The class setup puts each key spell on the button of its keybind category, now including Shield Wall, Hammer of Justice, Freezing Trap, Frost Nova and Ice Block.
- Cooldown rows show the key of another rank of a spell when that rank is on your bars, and spell buttons on the Consumable Bar, mounts included, show their cooldown without a global cooldown swipe.

#### Fixed

- The zone ability's options, its box in move mode and its Blizzard UI switch name only the zone ability, and keybind mode no longer offers a key for an extra action button, which WoW: Forever does not have.

### Talents and spells

#### Improved

- The Planner row on Blizzard's talent window stays inside the window on small screens, and the Talent Planner tells you when Improve for Spellbook and talents is off.

#### Fixed

- The Talent Planner, the Training tab and the spellbook skin go on and off together, whatever order you turn them on in.
- With the game's gamepad interface on, EldoUI's buttons on the talent window, the spellbook and the trainer window step aside, and they come back when you switch to mouse and keyboard.

### Info Bar

#### Fixed

- The Durability info text shows its repair icon again.

### Tooltips

#### Improved

- On the Tooltip page, a row whose module or switch is off is grayed and says why.

#### Fixed

- Hovering an aura on an enemy nameplate in combat no longer causes an error with the smart tooltip position.

### Journal

#### New

- My Adventure keeps every dungeon and raid run with who was in it (name, class, level and role) and its loot rolls: who won which item and everyone's roll. Battlegrounds and arenas record nothing.
- Delete one run or one name from My Adventure with Undo. EldoUI never drops runs or companions on its own, and companion pages show what each companion won while grouped with you.

#### Improved

- Long run lists open one page of 100 runs at a time, and a journal with years of runs opens as fast as a new one. Runs and the people you ran with take about half the saved space, with nothing lost.

#### Fixed

- Forgetting a character in the Alts window backs up its journal first and says so, and the newest backup of your runs from before an update is no longer pushed out by later restores or imports.
- The Attunements tab no longer lists WoW: Forever dungeons without a quest chain as empty pages; such a dungeon shows up once you have taken one of its quests.
- On a German client, quest objectives in the Loot Guide show in German.

### Map and minimap

#### New

- The Vanilla Original skin puts the game's own classic border around a round minimap, scaled with the map.

#### Improved

- Show unexplored areas works from your first login: the parts of every zone you have not explored yet show dimmed, even where none of your characters has been.

#### Fixed

- Corner buttons on a small minimap no longer overlap.

### Windows and skins

#### Improved

- Turning a window skin or the Mail module off puts Blizzard's look back at once, without a reload: spellbook, professions, quest and gossip dialogs, mailbox, friends, guild, calendar, PvP, the game menu and addon option windows.
- Option gear panels, the Recent changes list, the setup's questions and help, the dungeon map and the journal's quick note share the look of EldoUI's other windows, and Escape closes the front one first.
- Text sizes, tooltip titles and tooltip text match the rest of the interface in every window.

#### Fixed

- Switching profiles or themes shows the new colors and skin right away, without a reload.

### Notifications

#### Improved

- Alerts, the zone toast, rare cards and the low-mana note on a ready check share one queue: they no longer pile up, a repeated alert shows once, and alerts that waited out a long fight drop away.

### Other addons

#### Improved

- The Other addons step in the setup lists only the addons EldoUI has a profile ready for, for your layout or specialization.
- Changes EldoUI makes to Questie, RestedXP or Guidelime settings ask first, name the profile and the characters that share it, and can be undone. RestedXP's new guide window is placed on the layout's guide spot with its step list.

### Options

#### Improved

- Turning a module off or switching profiles asks for a reload only when a module really needs one, naming only the Blizzard parts that do. Switching a module on and off during a fight switches it once, after the fight.

#### Fixed

- While the quest tracker is hidden by its Hide switch or its box, its visibility settings are grayed out and say why.

### Performance

#### Improved

- Bags, the vendor, the auction house, loot rolls, the Encounter Timeline, the Farming bar, Enemy Spotter, gathering pins and map coordinates redraw only what changed, and their timers run only while something is on screen.
- Cooldown rows, tracking bars, the cooldown pulse, the cursor ring, the Consumable Bar and the global cooldown bar share one cooldown reader, so a burst of cooldown changes redraws them once.
- Countdown bars, the ping feed, buff reminders, weapon enchant timers, minimap note pins, the quest tracker, waypoints, the Split Timer, Quickdraw and ActionCam work only while they show or are in use. Background work pauses in combat.
- The Loot Guide and waypoint arrows work out map positions with much less memory churn, Loot Guide search and the PvP page open faster, and the Loot Guide's side list waits until you open the window.
- Backups of a long journal and of years of runs are written a little at a time, so logging in after an update stays smooth.

### Saved settings

#### New

- Every update first keeps a copy of your settings and journal. The new Saved data page (or /eui data) puts a copy back, lists what a restore replaced so one click undoes it, and keeps any saved value EldoUI could not read aside instead of deleting it.

#### Improved

- EldoUI records which version saved your settings. After an update every profile is brought forward without removing anything, settings you never changed keep the value you saw, and one chat line tells you.

### Localization

#### New

- EldoUI's own texts are available in Danish: pick Dansk under General > EldoUI language and reload. Game words players say in English, such as quest, loot and raid, stay English.
- The setup's first step lets you pick EldoUI's language, with the same flags as General > EldoUI language, and offers the reload right away.

#### Improved

- General > EldoUI language shows each language's flag. The Danish texts come in a folder of their own that loads only when you pick Dansk, so playing in English uses no extra memory for them.
- With Dansk picked, menus, lists and window titles that still showed English now show Danish too, and so do the What's New page and the update note.
- A name font you pick no longer replaces the font of Cyrillic, Korean or Chinese names, and name fonts stay in place when you change the theme font.
- The newest Loot Guide texts, such as run backups and loot rolls, are translated into German, French, Spanish, Portuguese, Russian, Korean and both kinds of Chinese.

### General

#### New

- Mage Travel, the Party Quests panel, the Split Timer and the waypoint arrow can be set to show only in combat, out of combat, on mouse over or in a group, like the other HUD pieces.
- /eui probe textures lists which original interface textures your game client ships, ready to copy into a bug report.

#### Fixed

- Game windows, tooltips, nameplates, chat bubbles, the Training window and the Cooldown Manager no longer cause an error when the game hides a frame's layer or state from addons.
- Frames that fade out no longer cause an error when the game hides one of their parts from addons.
- Camp Helper recognizes every camp feature, the Anarchist's Workbench, Cookie's Feast and Iron Oven in any game language the first time you see them.
- The camera no longer swings back and forth when you close one NPC window and open the next.

### Classes

#### New

- **Mage:** Mage Travel has five style presets: Standard, Small, Large, Quiet and Out of combat.

#### Improved

- **Shaman:** Totem timers kept with the totem bar move under or beside it when the cooldown rows fill the space above it, and tick only while a totem is out or an imbue runs.

#### Fixed

- **Paladin:** The blessing reminder, the Blessing Plan and the ready check report count only the blessings that share the blessing slot on WoW: Forever, so Salvation no longer counts as one, and Blessing of Sanctuary and Sanctity Aura are gone.
- **Shaman:** Water Shield and Rage of the Farseer work on the cooldown bar, the shield reminder and the class setup, Fire Nova has a ready icon, and Windfury and Flametongue Totem show on the party squares.
- **Shaman:** The totems and Earth Shield that WoW: Forever removed are gone from the pickers, and a saved pick of one goes back to the first one you know.

## [0.6.6005] - 2026-10-18

The versions from 0.5.0 to 0.6.6005 in short: what they brought that is still in EldoUI.

### Setup and profiles

- A step-by-step setup with Express, a class setup for every class, a last page with "Revert this" for each change, and a once-per-login reminder for an unfinished setup.
- Preset packs (Modern, Classic, Vanilla, Healer and Minimal), UI amount (Essential, Moderate or Full), the Overview page with complete looks, and look strings to share.
- Imports of EllesmereUI, ElvUI and Edit Mode strings, and an ultrawide safe area.

### Layouts and move mode

- Move any frame with /eui move, hide a box with a right-click (a "Lock right-click" switch and a Hidden boxes page bring it back), and set keys with /eui kb.

### Unit frames

- Unit frames with Blizzard element switches, heal prediction, text tags and cast bar effects, unit-frame graphics (Vanilla rings, Portrait Bars or the flat look), and a class resource bar with the five-second rule.

### Group frames

- Party and raid frames with main tanks, group pets, raid sizes and click casting.

### Action bars

- Eight action bars plus pet and stance bars, with fade and visibility rules, Fill order, proc glow and Masque, and keybind presets with a preview before any key changes.

### Talents and spells

- The Talent Planner with Import build, pick order and a level-up checklist, Training with what your trainer teaches now and soon, and lower spell ranks lit on your bars, with Check ranks on the spellbook and /eui rankcheck.

### Info Bar

- The Info Bar with datatexts and a Dashboard, the error log (/eui errors) with a Report button that leaves out your character's name, realm, guild and chat text, Rare Scanner, the Encounter Timeline, Raid Tools with /eui pull, Combat Text and the Cooldown Manager.

### Chat

- Saved history, search, keyword alerts, a spam filter, per-channel colors, and guild roster lines folded into one.

### Tooltips

- Spell tooltips can show damage or healing per second and per mana, and the target or focus cast bar shows the spell's tooltip.

### Bags and loot

- Bags and bank with your other characters' items and sections you can fold, merchant restock lists, the Loot Guide with best-in-slot sets and a wishlist, Raid Loot, Appearances and Farming history.

### Journal

- My Adventure, a journal of your road from 1 to 60 told as a story, with backups and exports, and Attunements with raid keys, dungeon chains and class quests.

### Map and minimap

- Dungeon Routes, Map Notes with the rares you met, Transport Maps, addon minimap buttons gathered behind one button, and a slim button rail.

### Windows and skins

- Eight skins for the whole UI (Minimal Modern, Vanilla Original, Vanilla Refined, Warcraft Parchment, Forged Metal, Portrait Classic, Faction Heritage and Arcane), the Appearance page, panel tint, and skins for Blizzard's own windows.

### Notifications

- Alert toasts with your choice of sound, the level-up card, the Ready Check Report and class reminders.

### Options

- The Blizzard UI page with one switch per part of Blizzard's UI, the Visibility page with HUD presets, Recent changes with Undo, profiles that follow your character, talent group or content, and Large text, a High contrast skin, color-blind safe colors and sound cues.

### Localization

- The Loot Guide in German, French, Spanish, Brazilian Portuguese, Russian, Korean and Chinese, and player names in Cyrillic, Korean and Chinese show their letters.

### General

- The Profession Planner, Finder, Macro Editor, Fishing, Streamer Mode, the Split Timer and Hardcore death alerts.

### Classes

- **Mage:** Mage Travel lists the teleports and portals you know, and a mana gem button joins the Consumable Bar.
- **Paladin:** The Blessing Plan (/eui blessings) plans which blessing each paladin keeps up on each class.
- **Shaman:** Shaman Totems: a totem bar, a cooldown bar with your shield, weapon imbues, Reincarnation and Ankhs, up to eight totem loadouts, and a group plan for Mana Tide Totem and the resistance totems.

[Unreleased]: https://github.com/Eldodeldo/EldoUI/compare/v0.7.1000...HEAD
[0.7.1000]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.1000
[0.7.0003]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0003
[0.7.0002]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0002
[0.7.0001]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0001
[0.7.0000]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0000
[0.6.6005]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6005
