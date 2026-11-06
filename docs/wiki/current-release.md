# Current release

<!-- eldoui:release-docs 0.7.1000 -->

EldoUI **0.7.1000**, 2026-11-04.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.1000) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.1000/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

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
