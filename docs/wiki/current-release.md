# Current release

<!-- eldoui:release-docs 0.7.1001 -->

EldoUI **0.7.1001**, 2026-11-06.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.1001) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.1001/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Layouts and move mode

#### Fixed

- The zone toast sits under the ready check, clear of the alerts beside it, also with Notifications off. The ready check moves up a little and the countdowns move above the spell alerts. Modern Center, Portrait Staggered and Nameplate Focus stay as they are.
- On 16:10 screens, bigger action bar buttons, a larger minimap, wider unit, party and raid frames and a wider micro menu no longer push frames on top of their neighbors.
- On 16:10 screens, the boss info box, the raid warning, the loot toasts and, in Close Combat and Nameplate Focus, the ping feed get their own spots where they touched a neighbor.
- On 16:10 screens, Portrait Staggered's extra ability button sits a little lower and Vanilla Original's target of target a little higher, clear of their neighbors, also with bigger bar buttons.
- On 16:10 screens, the Battle.net toasts stay clear of bigger action bar buttons in Close Combat, Compact HUD, Open Center and Modern Center, of wider player frames in Widescreen Edges and of wider party frames in Nameplate Focus.
- On 16:10 screens, the death recap in Twin Orbs stays clear of the boss frames.
- In Vanilla Original, popup dialogs open below the top notices with the Clean, Healer, Perl or Portrait unit frames, so they no longer cover the target or the target of target.
- The Blizzard-like layout no longer offers the large action bar buttons: on 16:10 screens they pushed bar 4 over the game's micro menu row.
- Leaving Twin Orbs no longer leaves your health and power orbs stacked in a corner. The orbs stay with Twin Orbs and your player frame takes the new layout's own style, also when you keep your look. The layout question says so first.

### Gamepad

#### Improved

- The Classic movement key set puts bars 1 to 3 on 1-5 R F G V X Z C, with Shift for bar 2 and Ctrl for bar 3, so T is free and V is used. The Consumable Bar keys move to Ctrl + X, Z and C. Take the set again to get the new keys.

#### Fixed

- Check my keyboard in the key set window highlights the key to press without a Lua error.
- Show the changes on the spell rank prompt opens the key set window without a Lua error.
- Apply and Undo last Apply in the key set window no longer freeze the game or stop half way while the window is open.

### Unit frames

#### Fixed

- Player names in Cyrillic, Korean or Chinese show their letters on the target frame and every other unit frame instead of empty boxes, also on the game's own frames when EldoUI styles them.
- Resource bars and a detached player cast bar set above or below the cooldowns keep their spot and keep updating while the cooldowns can't be measured, and sit on their own mover when there is no cooldown row.
- A detached player cast bar set above or below the cooldowns takes its place on the cooldown stack again, past the resource bar, the item row and the tracking bars.
- With the name above the bars, as in Blizzard-like frames, the target of target and the pet frame sit above the target's and your own name with a clear gap instead of covering it. A frame you dragged stays where you put it.
- The target of target never rises over the game's totem bar when you move that bar.

### Group frames

#### Fixed

- Names and health values on light class colors, such as a priest's white, a mage's light blue or a paladin's pink bar, get a thick dark outline and shadow, so they read on the bar and on its empty part, whatever your font outline setting.
- Pet frames, and any group frames with their auras turned off, no longer set aside aura icons they never show, so they use less memory. Turning their auras on adds the icons as before.

### Nameplates

#### New

- The Game settings tab of the nameplate options has a Plate distance slider. It shows how far plates reach now and gives you the chat command for the distance you pick, ready to copy, since the game lets only you change this setting.

### Action bars

#### Fixed

- A click on a Consumable Bar button uses its item again when the game casts on key press, and its keys work on the press. Pet feeding, fishing, raid tool, travel, bag action and quick menu buttons act on a click the same way.
- Picking up or placing a spell during combat no longer shows "Interface action failed because of an AddOn" when EldoUI's bars replace the game's extra bars.

### Auras and cooldowns

#### Fixed

- The Healthstone reminder shows only when you or a warlock in your group can make one, so a warlock who has not learned Create Healthstone yet is no longer asked for one.
- The boss-mechanic aura slots next to your debuffs follow your settings again after a layout that couldn't finish, without a reload.

### Combat

#### Fixed

- The damage meter skin no longer causes a Lua error at login while the meter still shows rows from a fight.

### Info Bar

#### Fixed

- The Gold readout counts from your first coin. With less than one gold it shows your silver and copper instead of 0, in the Gold only and short formats too.

### Chat

#### Improved

- The chat setup keeps everything in your main chat window, also with the Whispers, Loot and Channels tabs: experience, honor, reputation, currency, tradeskills, pet and target icon lines, channels and whispers show there too. Run the chat setup again to add them.
- A whisper window shows the contact's name in their class color and their race and class under it, also for players outside your friends list and guild. Their level shows once the game has seen it (group, target, mouse-over, nameplates) and stays for the session.

#### Fixed

- Whisper windows, their history and the chat message line show names and messages in Cyrillic, Korean or Chinese with their letters.
- Shift-clicking an item, spell or quest while you type in a whisper window puts its link in the window's message line at the cursor, like the game's chat box.
- Player notes, chat levels, guild mutes and Streamer Mode recognize players who have a surname, and a note saved under the surname moves to the right player.

### Bags and loot

#### Fixed

- The bank's buy-a-tab button no longer changes during combat; it updates as soon as the fight ends.
- The merchant's All items grid opens and refreshes again when a price or stock text has a fractional width.

### Leveling and quests

#### Fixed

- The Party Quests panel moves when you drag its title and keeps the new spot.
- The Party Quests panel opens in the top left, clear of the quest tracker, so the two lists no longer show through each other. Modern Center, Portrait Staggered and Nameplate Focus keep the spot they had.
- In the healer setup of Blizzard-like, Hunter and Sanctum, the Party Quests panel opens a little higher, so it no longer covers action bar 8.
- The quest tracker's +/- button sits on the tracker's own top row, next to its fold arrow, so it no longer covers the word "Total" on the Split Timer under the minimap.

### Map and minimap

#### Fixed

- Continent and world maps show only Transport, instance entrances and your own notes, so they are readable again. Zone and city maps show everything. Map Notes has an Also on continent maps tick for each group; City services stay on zone and city maps.
- Turning the minimap off during combat keeps it off after the fight, instead of EldoUI's minimap coming back.

### Windows and skins

#### Fixed

- The friends, guild, who and group finder lists, the damage meter and the death recap show names in Cyrillic, Korean or Chinese with their letters.
- The side tabs in the character window show their own icons whole and at the same size, inside an even border. The Titles and Equipment Manager tabs no longer show cut-up pieces of other art.

### Notifications

#### Fixed

- The ready check, its countdown and the dungeon-ready timer show at the game's own spot with no Lua error when their EldoUI position can't be read.

### Other addons

#### Fixed

- Turning an addon's layout spot off and on again during combat keeps your last choice after the fight, instead of sending the addon back to its own spot.

### Options

#### Fixed

- The frame preview on the Unit frames page always fits inside its strip, shrunk with its shape kept when the frame is large, so it no longer covers the settings below it. A power bar or orb on its own position is no longer drawn under the frame in the preview.

### Saved settings

#### Fixed

- Put back on the Saved data page waits until you are out of combat, like Restore backup and Undo restore.

### Localization

#### Fixed

- The Text tags tab on the Lists and tags page shows in Danish too.

### Classes

#### Improved

- **Shaman:** Right-click the shield or a weapon imbue icon on the Shaman Cooldowns bar to pick which one it casts, such as Rockbiter, Flametongue or Windfury. The menu lists the ones you know and works out of combat.

#### Fixed

- **Shaman:** Picking an Earth or Fire totem on the Shaman Totems bar sets it in Call of the Elements again. Before, the game refused it with "Only Fire Totem spells can go in that slot", because the two slots were swapped.
- **Shaman:** The tooltip of the Shaman Totems bar opens beside the bar, so it no longer covers the totem lists that open above the buttons.
