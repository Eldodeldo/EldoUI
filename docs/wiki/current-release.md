# Current release

<!-- eldoui:release-docs 0.7.3000 -->

EldoUI **0.7.3000**, 2026-11-16.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.3000) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.3000/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Highlights

- Flight Games is on by default and the Games box appears on your next flight path.
- Auto UI scale keeps the full layout width on 16:10 screens.
- Move mode can undo your last change and keeps locked frames in place when you reset.
- Profile resets, copies, deletions, and imports keep a backup you can undo from the alert.
- Choose group quests and dungeon routes separately for each character in the leveling guide.
- Bag and bank windows share the same look and stay sharp at any window scale.
- Dungeon bosses in the Journal learn their drops from group and solo loot.
- The Alerts tab keeps its lines between sessions and follows your EldoUI language.

### Setup and profiles

#### Improved

- The setup step that imports EldoUI profiles into your other addons is now Addon profiles, so Other addons names only the options page.
- The Styles, Keys and spells, and All set steps open with two short sentences each, and every button and description calls it the setup, as in "Run the setup again".
- Resetting, copying over, deleting or importing into a profile keeps a copy first, and an alert offers Undo or Keep. The copy also stays on the Saved data page.
- The questions before a reset, copy or delete name the other characters that use the profile, say what happens to them, and say when the setup opens again.
- The one-click pack names the other addons it turns off before you press Apply.
- /eui setup opens the EldoUI setup like /eui install, and the new /eui addonsetup names the addons it writes profiles into and waits for your Yes.

#### Fixed

- Undoing the last setup in combat says it runs when combat ends, and typing /eui install several times in combat opens the setup once afterwards.
- Undoing a profile deletion restores the Otherwise use choice and the profile you return to after leaving a group, while keeping choices you changed afterwards.
- Undo setup works on the profile under its new name after a rename, and never brings back a profile you renamed or deleted.
- On a new or reset profile, Group frames set to Blizzard frames, untouched and Nameplates set to General colors keep that choice after a reload.
- Copying or importing General settings keeps your layout. A new Layout choice brings the other profile's layout, with its frame sizes.
- When the Keys step can't set your keys (a spell on the cursor, or keys changed since the preview), the setup stays on that step with the warning and no longer says the keys were applied.
- The Welcome page now explains how to set up another profile instead: switch to it on the Profiles page, and the setup starts over there.
- Undo the setup turns the addons the setup turned off back on, and its question names them.
- With profile rules on, a profile you pick yourself stays until your content or talent group changes, leaving a group goes back to the profile you were using, and a new Otherwise use choice covers everything no rule fits.
- Importing a string from a newer or an unreadable EldoUI, or one that needs a layout you don't have, now says so instead of calling the string damaged, and an export that can't be made names the part and the reason.
- All frame positions, as a share string or copied from another profile, now also brings the places and sizes of the game windows you dragged. Strings made before keep your windows where they are.
- Undo setup on a profile the setup made finishes again: you are back on your earlier profile and get the prompt to reload.

### Layouts and move mode

#### New

- Undo last takes back your last change in move mode, one step at a time: a drag, a nudge, a typed position, an attach or a reset. Ctrl+Z does the same.
- A key binding opens and closes move mode (Key Bindings, AddOns, EldoUI).

#### Improved

- The move panel names the point a position is measured from in words, X, Y, Grid and the arrows explain themselves, and a box without a number shows its value again.
- A frame dragged against the edge of the screen now sits flush on it.
- Reset all in the move panel asks first, and frames you locked keep their place. Shift-right-click no longer resets a locked frame.
- Dragging stays smooth with many boxes on screen, and the grid follows a new UI scale or window size while move mode is open.
- On a 16:10 screen the Auto UI scale keeps the full width every layout was made for, so the frames sit as they do on 16:9 with a little more room between the top, the middle and the bottom of the screen.

#### Fixed

- Raid Tools has room beside the enemy spotter and counters in the built-in layouts.
- A fight that starts during a drag ends the drag where the frame is and keeps that place, instead of leaving the box stuck to the cursor.
- Combat now says why move mode closed and opens it again after the fight, with Undo changes still able to put everything back.

### Unit frames

#### New

- Optionally show your interrupt's icon and cooldown while your target or focus casts.
- Quest icons on your target and focus show mobs needed for your unfinished objectives.

#### Improved

- The player's PvP badge can show when your PvP flag expires, with the same countdown in its tooltip.
- Test frames show sample buffs and debuffs in each block's size, rows and direction, and every boss frame shows its sample cast bar, so spacing can be judged without a target.
- Health and power texts have their own size and can be nudged on each frame, so the health number can be larger than the name or moved off an edge. The defaults look as before.
- The layering setting in the gear is now Stacking order, and its description says when to change it.
- Cast times on the unit frames count in tenths of a second, like the nameplates, and the spark and channel ticks stay crisp at every scale.

#### Fixed

- Cast bars under the unit frames line up with the frame's edge to the pixel, and the spell icon shares one border line with the bar.
- A centered name no longer runs under the health text, and a name beside the bar uses the whole bar when health text is off.
- Test frames show what the real frames would: hidden texts stay hidden, texts follow their format, the player frame carries your name and class color, and the sample cast follows the time format and cast color.

### Group frames

#### New

- An optional healer mana list shows class-colored names, mana bars, and your chosen raid or party healers.
- A Loot button on the Raid Tools bar shows the loot method, the master looter and the threshold. The group leader clicks it to pick the method, the master looter or the threshold; everyone else sees what the leader set, and a line in your own chat can tell you when it changes.

#### Improved

- The ready check report shows when a group member is eating or drinking and leaves them out of the missing-food count.
- The member who hands out the loot under master loot gets the game's master looter mark next to the leader crown. It moves when the leader picks someone else and can be turned off under Indicators.
- The Ready Check Report shows a thin bar with the time left to answer, and after the check one line in your chat says who is ready, who said not ready, who never answered and who is offline. By default only a leader or assistant sees it, and Post to group sends it on a click.
- The role icon can leave out damage dealers so only tanks and healers stand out, and sorting by role can put healers before tanks.
- The world marker buttons on the Raid Tools bar light up while their marker is on the ground and dim when it is not, and the tooltip says Placed or Not placed.
- Party and raid frames light up under the mouse in the same soft white as the player and target frames, so frames side by side look alike.

#### Fixed

- Where the game lets EldoUI read a debuff, the dispel highlight and glow stay off for debuffs on the Never show list, following the debuff row's Use the Never show list switch.

### Nameplates

#### Improved

- The health text can sit left, center or right in the bar and has its own size per plate type. By default it gets smaller on a thin bar so it stays inside.
- Stack and countdown numbers on plate auras grow with the icon, so they no longer cover a small icon or get lost on a large one, and the Auras tab can set both sizes.
- The three mode buttons say what you see after a click, the Overlay and Pulse glow highlights explain themselves in the list, and the color order says which color wins.
- Name-only plates show your target with a line under the name in the target color, and a lighter line on the plate under the mouse.
- The slim styles Twilight slim and Whisper use smaller raid marker, crowd control, elite and quest icons that fit their thin bars.

#### Fixed

- Buffs beside the bar and the target arrows sit next to an ordinary mob's bar, with room kept only for the elite, quest and pet icons the unit has, and both arrows the same distance out.
- Your target's plate keeps sharp one-pixel borders at its larger size.

### Action bars

#### New

- Choose whether right-clicked actions on EldoUI bars use their normal target or your character.
- An Active look setting picks how a button shows an active stance, Auto Attack or a toggled spell.

#### Improved

- Macro names have a position setting on the Text tab and in each bar's own text settings. If the count shares the macro name's row, it moves clear of the name and the keybind.
- The Auto Attack and Auto Shot pulse, the glow on a newly placed spell and the spellbook hover highlight follow the button's shape.
- Pet and stance buttons use the bars' cooldown numbers and Icon zoom, and the preview and move-mode stand-in show each bar's button shape, growth and fill order.
- Your other characters (Ask me, Automatic, Off) can now be changed on the Keybinds page, and the New spells choice uses the same words.

#### Fixed

- The hidden vehicle seat picker no longer catches mouse clicks.
- Keybind mode keeps keys character-specific until you confirm sharing them across your account, including when combat starts or the window closes.
- /eui kb classic opens Classic movement, a key set's name works after /eui kb, and /eui keybind, keybinds and bind open keybind mode. The key notice says "One thing" when only one thing is in the way, and the preview says how to use a key set while you manage your own keys.
- Button borders stay one sharp pixel on a bar scaled above or below 100 %.
- Lock action bars no longer jumps back to an old value after you change it in the game's options.
- A bar at 0 % opacity takes no clicks and shows no tooltips.
- The pet and stance bars follow the Text tab at once, without a reload, and small buttons get a keybind that fits.
- Show the keys on bars 1 to 3, from the setup or the key set alert, can now be turned off again on the Keybinds page, and Show keybind says when it applies.
- Undo last key set leaves keys you changed by hand since alone, asks first on the Keybinds page, and has one name everywhere.
- Key set confirms say when your keys are shared by your account, keybind mode asks before saving one character's keys for the whole account, and a bound key names the action it was taken from.
- Spell cues light Judgement and its own button for Seal of Fury, and Aspect of the Beast glows on its button while it is up.

### Talents and spells

#### Fixed

- The level-up card no longer lists ranks of talents you don't have, and its training cost is right.

### Auras and cooldowns

#### New

- Buff and debuff tooltips say who cast them: you, a group member, your pet or theirs. The line stays away when the game keeps the caster hidden.
- Pick the spell and rank each class buff reminder asks for: the imbue per hand, your armor, aspect, aura, seal or blessing. Right-click the icon or use the Class buffs page; by default it follows what you cast last, at your highest rank.

#### Improved

- Buff and debuff tooltips open toward the free side of the screen, and the weapon enchant icons follow each style preset with the debuffs.
- The buff and debuff preview follows every stack and time setting: stack size and place, time place, the time bar and grayed buffs from others.
- The Debuffs tab no longer offers Yours first and Gray out others', which grayed out nearly every debuff from enemies.

#### Fixed

- The time text under a buff no longer sits on top of the time bar.
- On the Blizzard tab, Scale and Time left under Blizzard's buffs are grayed out while their Move or Improve switch is off.
- Blink when expiring blinks visibly with Swipe with numbers, which now shows one countdown per icon, and Color by time left is only offered where it applies.

### Combat

#### New

- Hold Shift before releasing your spirit in a dungeon or raid with an optional safeguard.
- Instances can automatically start combat logging in raids or in raids and dungeons.
- Nemesis keeps a history of opposing players, lets you rank them on a personal priority list, and can alert you outdoors after three confirmed kills in either direction.
- In battlegrounds, a Next resurrection bar at the top of Battleground Timers counts down to the spirit healer's next wave while you wait, in your faction's color, and goes when you are back.

#### Fixed

- Open Nemesis history updates as soon as the game confirms who killed you.
- The Class Bar offers WoW: Forever's new cooldown abilities and counts teleport runes and Light Feathers once their spells are learned.
- Right-click a cooldown on the Class Bar to choose its spell rank for each character, or let it follow the highest rank you know.
- A full Class Bar starts a second row after 10 icons, so a paladin's or mage's bar no longer hangs over the player and target frames; Icons per row sets where it wraps.
- A combat text event's sound plays when its line appears, and a burst of lines with the same sound plays it once.
- A new custom combat text area always starts at its default place, also after deleting a dragged one with Gamepad Mode UI on.

### Info Bar

#### New

- Shift-click the Zone or Coordinates block to put your location into the chat line you have open.
- The Time and Date tooltips list waiting calendar invites, today's events, the next guild event and the reset countdowns, and both blocks show a dot while an invite waits. The Guild tooltip names the next guild event.
- A Group block shows the group size, how many tanks, healers and damage dealers it has and who is offline. Its tooltip shows the leader, assistants, loot method and master looter and lists the raid by group. Click opens the raid panel and right-click opens Raid Tools options.
- A Lua errors block counts the new entries in EldoUI's error log, lists the newest in its tooltip and opens the log on a click. It takes no room while nothing is new.

#### Improved

- Every block you can click lights up under the mouse with the same soft hover as other controls, the » button too, and the Currencies, Item level, Custom currency, Reputation and Played tooltips say what a click does.

#### Fixed

- The Durability tooltip includes repair costs for damaged items in your bags.
- The gold, hearthstone and rate tooltips show their gains, losses and cooldowns in the color-blind safe colors when those are on.
- The hearthstone panel no longer shows an error when the game keeps the item count hidden.

### Chat

#### New

- The optional Trade board keeps recent public chat offers in one searchable window and opens a whisper draft when you click an offer.
- An optional setting invites players who whisper your exact keyword when you are out of combat. It is listed with the other conveniences in the setup and on the Conveniences page.
- An optional setting adds Guild invite and Who to player right-click menus.
- Hide system messages about learned and unlearned spells with an optional chat filter.
- Right-click a channel name to leave it from the menu, when the channel allows leaving.

#### Improved

- Chat filters preserve friends and group members, can include whispers from strangers, and recognize disguised repeats and blocked phrases.
- Instant Messages can forget old conversations after a number of days you choose.
- An optional setting shows the equipment slot and armor or weapon type inside gear links.

#### Fixed

- The Alerts tab keeps the same window and saved history when you switch languages.
- The "1/3" part counter and the length counter sit just above the chat input, so they no longer cover the emoji button or the last letters you typed.
- A chat bubble the game draws a moment late gets the EldoUI style right away instead of keeping the parchment until the next line.
- Lines in the Alerts tab have one timestamp, the clickable one, when EldoUI timestamps are on.
- The Alerts tab and its source labels follow EldoUI's language, so a Danish tab is named Advarsler.
- Item icons on chat links keep coming during a long session, instead of stopping after the first hundred items the game had to load.
- Save whispers off now keeps every whisper out of the saved history, also its copy in the right panel and whispers restored from an earlier session, and deletes the whispers saved so far.
- The Alerts tab keeps its lines between sessions like every other tab.
- A line the chat hides (blocked phrases, channel mutes, repeated lines, a muted guild) no longer plays a channel, whisper or keyword sound or flashes the taskbar, and a channel no chat tab shows stays quiet.
- Setting timestamps or class-colored names back to Keep game setting, or turning EldoUI timestamps off, brings back the game's own setting.
- The whisper sound of Instant Messages follows No alert sounds in combat and plays at most once every 2 seconds.
- The Invite and Add friend buttons in a whisper window leave confirmation to the game, so a refused request does not show a success notice.
- The rest of a long whisper to a player with a surname goes to that player, not to the first word of the name.

### Tooltips

#### New

- Trainers, weapon masters, vendors and flight masters say what they have for you: the spells your class trainer can teach you now and their cost (or the level where the next one opens), the weapon skills you lack, the recipes you can learn, and a flight path you have not learned.
- An item a quest in your log asks for now shows that quest with how many you have and how many it needs, and turns green once you have them all. The Loot Guide's "Needed for" row no longer repeats a quest named there.
- Herb and ore tooltips show how much of the gathered item you carry and how much your characters have together.
- Opposing players' tooltips show how many times the game identified them as the player who killed your character. The count carries over between logins.
- Player tooltips mark your friends, members of your own guild and players you ignore, out of combat.

#### Improved

- Tooltips can show compact item stat lines, including the items compared beside them.
- Auction prices show the usual price from your saved searches and say when a vendor pays more. Hold Shift to see the last seven days.
- Auction prices in the shared tooltip row show the total value of a stack alongside the price per item.
- One Show IDs choice covers item, spell, aura, NPC, quest, currency and object IDs, and friendly NPCs show their ID too. Your earlier Item ID and Spell ID choices carry over; when they differed, the stricter one is kept. With Shift, stackable items show their stack size.
- Options that need the Skin or Move switch for Blizzard's tooltips are grayed while it is off and say which switch to turn on, and Scale now sits with the other look settings.

#### Fixed

- The safe-to-sell line on gray items stays out of the way when the game withholds an item's quality or sell price.
- An item whose Value row holds an auction price says "Value" instead of the game's "Sell Price", and every price in a tooltip uses the same money style; the auction window's "Prices as" setting now applies to the window only.
- A guild name with the word "Level" in it keeps its own color, and the player's real level line gets the level color.
- With Hide in combat on, a tooltip for an item link you clicked stays open, and so does the comparison beside a tooltip you choose to show.
- The Hold to show in combat key brings a hidden tooltip back at once, even while you keep pointing at the same thing.

### Bags and loot

#### New

- Raid Loot can record who attends each boss and raid night, keep a bench list, and copy attendance as text or CSV.
- The selected profession recipe shows estimated skill-up steps, crafting costs, sale values, and available crafts, with a button to list missing reagents.
- Bag and bank tooltips show their value, and nearly full bags mark a low-value stack that the loot window names when you run out of room.
- Mark junk in your bags and bank, then sell up to twelve stacks with one vendor button click.
- Find auction deals in your searches and full scans, set watch prices, and see a warning before listing an item far below its usual price.
- Bound loot that you can still trade shows the minutes remaining in its bag slot.
- Search bags and saved items by tooltip text, required level, recipes and collectibles you know, or gear upgrades.
- An optional solo-loot setting confirms Bind on Pickup items while you loot alone.
- Choose whether new loot goes into your first or last bag, or keep the game setting.
- Choose to close open bags when combat starts, while keeping bags you open during combat available.
- Merchant can limit automatic junk selling to one batch of up to 12 stacks per visit.

#### Improved

- Bag and bank footers show free slots, warn when space runs low, and show each bag's capacity on hover.
- Bag cooldowns refresh together during bursts, and Shaman totem coverage ignores unrelated units.
- The character window's item level setting also shows item levels in the ring, trinket, and Alt-hover equipment menus.
- Junk coins and dimmed icons in your bags follow Merchant's sell and keep rules, including protected items.
- The bag and bank windows use the same title, edge, accent line and text styles as every other EldoUI window, and stay sharp at any window scale.
- Junk coins, lock marks and set marks grow with the slot size.
- The sort button dims in combat and its tooltip says why, and settings that only work in the Categories view say so when another view is picked.

#### Fixed

- Skill-up notices recognize both of the game's message formats.
- Bag space totals and Info Bar warnings count general slots. Quivers and other special bags keep their own counts.
- Loot Guide includes one-handed axes when showing gear rogues can use.
- The auction window's Ledger style writes prices as letters as it promises, and Standard follows your general money style.
- The upgrade arrow no longer covers the item level, and gear you can't use gets one red mark in the bags, set by the bag window's own switch.
- Loot rolls appear when their item details arrive, including rolls with a missing icon, and canceled rolls stay closed.
- The crafting guide shows the updated cloth-bag capacities and material counts, and the Holy Power recipe's current name.
- The Loot Guide shows racial vendor mounts with the current bind-on-pickup rule.
- Learning a spell updates the usable marks in the bags and the green tint on known items at once.
- Glow on new items shows on every item again, also gray and white ones and with quality borders off.
- Fishing catches and made items whose loot line has no item link show in the loot feed with their icon and color, and Farming counts them.
- All characters search results stay on screen: a long list scrolls, the panel opens on the side of the bags with room, and Shift-click on a row links the item.
- The guild bank window follows the bag window's slot size, spacing, window size and Money style, shows No matches, and clears its search on close when that option is on.
- Every open group loot roll shows at once, with no limit of four. A roll that starts in a burst or right after a boss gets its own bar even if another roll's item details are still missing.
- The gear comparison only uses talents your class has on WoW: Forever, and counts Shredding Attacks for druids.

### Journal

#### Improved

- Boss rows show a check when you defeated that boss in your current lockout or run.
- WoW: Forever dungeon bosses learn their drops from the group's loot history and from the boss's loot window too, so group and solo kills fill in their pages. Each item counts once per kill.

#### Fixed

- A new kill no longer counts older loot rolls again when you defeat the same dungeon boss.
- Pasting a journal backup accepts the new compact codes. A code with only recent changes is merged into your journal.
- Importing an installed journal again keeps new moments recorded in the same second as the last imported moment.
- A level or new-place card shown on its own takes in its brief without sliding in a second time.
- "Clear this character's journal" now gives an empty journal. An older copy of the journal no longer comes back in its place, and the same goes for undoing an import.
- When a character takes its journal back from older copies, their notes, goals and moments come along too, not only places and dungeons.
- Two characters that once shared a name each keep their own journal backups. A backup of another character's journal can't be restored into yours, and a renamed character keeps its journal and backups.
- On game clients in other languages, each WoW: Forever dungeon shows once in the Journal and learns its bosses when you defeat them.

### Leveling and quests

#### New

- My Adventure's level cap milestone shows the XP left to the cap and about how long it takes at your pace, and milestone times weigh the XP each level needs. Rested XP and finished quests count as a head start.
- The XP bar tooltip shows the XP and time left to the level cap (option "XP to the level cap", on by default).
- Two key bindings cycle forward and backward through your tracked quests. The quest item button follows the selected quest when set to Super-tracked first.
- Copy the talents you have in either talent group as a loadout string from Talent Planner.
- Level difficulty colors have their own row on the Colors page, and the color-blind safe palette gives them a gray to vermilion ramp. With shape marks on, tooltips and the Training window add the level gap, such as +3.
- The Training window lists Apprentice Riding at 40 and Journeyman Riding at 60 with their cost, and the level-up list names the rank when it opens. Once you open a riding trainer, the cost it asks replaces the estimate.
- The XP bar tooltip lists each running XP bonus, such as XP food or an event, with its bonus and time left. An optional line on the bar shows while one runs, and an optional reminder says when no XP bonus is running while you level.
- Choose group quests and dungeon routes per character, with optional deathskips that stay off in Hardcore.

#### Improved

- Training skips unnecessary list updates when you change forms or enter a new area, and still updates when you learn a spell.
- Hold the game's comparison key (Shift by default) over a new rank in Training to see the rank you know beside it.
- Party Quests updates after quest progress and shows current cards as soon as you join a group.
- Community guides include the latest route corrections and new class and reputation guides.
- The quest tracker's Questie tab shows its settings only while Questie is loaded, and says so when it is not.
- The guide follows conditional route jumps and background objectives, with route choices preserved through Undo and reloads.
- Undo in the guide also takes back goals the game ticked for you, such as an arrival or a landing.
- The quest tracker's new-quest color and the color-blind difficulty word are drawn over the tracker's titles and leave the game's own titles alone, and a long title is shortened once instead of on every tracker update.

#### Fixed

- The quest tracker keeps your character's folded or open choice when you turn the Quest Tracker module off or on. EldoUI's fold button stays at the tracker's corner while it is folded.
- Quest tracker titles with difficulty words fit again when you change the font or text size.
- Once an "along the way" stretch of the guide ends, only its goals with work still open stay listed; finished lines and the accept line drop off.
- Completed money and arrival goals stay complete after spending or moving away, and Undo restores their earlier progress.
- The guide ticks "Get the flight path" only at the flight master the step names, and one flight ticks one "Fly to" goal, where it landed.
- On a turn-in whose open objectives have no known place, the guide's arrow keeps pointing at where you hand the quest in.
- A guide step you went back to stays after a reload, a search loop keeps its place, and a flight that was under way still counts when it lands.
- XP and reputation bars set to the full screen width follow a new resolution or UI scale right away.
- The XP bar tooltip shows rested and finished-quest XP in the colors you picked for the bar, and it opens below a bar at the top of the screen and beside an upright bar instead of off the screen.
- Folding the quest tracker with the per-character button or /eui tracker no longer leaves the game's tracker and Edit Mode reporting that they cannot read auras in combat. The folded tracker is set aside, and the button stays where it was.

### Map and minimap

#### New

- Open a see-through minimap in the center, keep your pins, and click through to the world.
- The flat tracking button shows the icon of the tracking you have on, such as Find Herbs or Find Minerals, names it in its tooltip, and dims while nothing is tracked.

#### Improved

- Show unexplored areas also works on the battlefield map when you let EldoUI change it.
- Map pins share their movement updates and stay still while you stand still or hide the minimap.
- The waypoint arrow keeps steady text while you stand still and smooths its arrival estimate while you move.
- Minimap pings briefly show the sender's name in their class color.
- The section for the map notes addon shows only when that addon is installed.
- The layer chip sits on the same readable plate as the zone, coordinates and clock, and the clock and the chip light up under the mouse.
- EldoUI's map pins draw in one fixed order on the world map and the minimap: gathering nodes lowest, then rares, services and entrances, quest givers, your notes and waypoints on top, all under the game's quest objectives and group members.

#### Fixed

- Closing the world map with Escape no longer blocks the game's quest pins or fills the chat with "Interface action failed" lines. EldoUI's waypoint, note, gathering, transport and unexplored-area layers now follow the map without joining the game's own pin list.
- The minimap steps back when another addon has its enhanced minimap enabled, keeping one owner for its position, shape and buttons.
- The minimap button drawer finds buttons from addons loaded later and collects them after combat.
- Zone tooltips list WoW: Forever's new dungeons with their level ranges, including entrances in Ironforge and Undercity.
- Repeated layer-hop requests from one player wait before another offer, and a burst of requests keeps the pending list bounded.
- Layer hop waits for the game's invitation popup and tries another helper when an invitation is refused.
- The minimap border and the XP bar ticks stay one sharp pixel after a UI scale or resolution change, and the high contrast art style gives the minimap its 2 pixel border.
- With the zone name on mouseover, it stays while the cursor is on the clock, the layer chip or a corner button, and above the map it fits the map's width.
- With the Maps module off, the world map no longer draws or saves unexplored areas.
- Note, gathering and waypoint pins on the minimap come back as soon as the indoor minimap or a hidden pin group gives way, without having to move.
- Clicking Add note several times in combat opens the note editor once after the fight, and the minimap settles once after combat instead of once per change.
- With Help others hop on, a hop request another player answers with someone else's help is forgotten after a minute, so a long session in a busy city no longer piles them up.

### Windows and skins

#### New

- The Guild window opens a local history and a filterable roster with last-online times, with optional main links in guild chat.
- Choose to show the remaining time on weapon oils, stones and poisons in the character window.

#### Improved

- The Alts window's Professions grid marks a skill at its cap only while a next rank exists, so 300/300 no longer reads as a warning.
- The class bar, totem, consumable bar, mage travel, pet feeding and fishing buttons share one hover and pressed look, so buttons side by side match.
- While the windows are locked, the drag, scale and reset keys on the Move windows page are grayed and say why.

#### Fixed

- The character window no longer marks librams, idols, totems or thrown weapons as missing an enchant, since they take none.
- Window skins keep the original artwork when the game protects it and restore it correctly when you turn a skin off.
- Quest and gossip windows, the group finder and other Blizzard windows no longer raise an error in instances when the game hides a frame's mouse state or icon from addons.

### Notifications

#### New

- The Hardcore death log has filtered zone, level and cause statistics, with optional notices about recorded deaths near your level.
- Fanfare can celebrate a completed quest objective or a quest that is ready to turn in, with effects you choose.
- When a profession reaches the top of its rank, such as First Aid at 75/75, one chat line names the rank to train so no skill points go to waste. An optional early line comes five points before.

#### Improved

- Danger Alerts can pulse your gamepad, and their alarm sounds stop after three seconds.
- The text size sliders for zone names, error lines and the talking head say what they size and show "Game size" at 0.
- The game's box that counts down to moving you to another layer now appears with the Battle.net toasts, above an open toast, instead of where the default chat used to be.

#### Fixed

- Rare alerts can place waypoints on the parent map when a marker has no position on the current map.
- At the level cap, the level-up sample in the alerts test shows your level instead of one past the cap.
- The title, text and sub line of an alert toast never overlap: the toast grows to fit its text at any icon and text size, the Minimal style included.
- Hovering an alert toast whose name is cut off shows the whole name.
- The reminder sound plays when a reminder first appears, not again after every fight, death, flight path or reload.
- A buff reminder set back to Automatic no longer keeps casting a lower rank you picked earlier.
- Shaman shield and weapon imbue alerts no longer pop while you are dead, on a flight path, or where reminders are set not to show.
- Leveling up inside a dungeon shows the level-up card with your new spells again, and a long spell list fits the card and stays up longer.
- Danger alarms for auras go quiet with Mute EldoUI sounds, and a debuff that lands again every tick sounds at most once every two seconds.
- The dungeon ready sound and taskbar flash no longer depend on the timer bar, a battleground pop sounds once instead of at every update, and the switch is now called Play a pop-up sound.
- Skip cutscenes you've seen now skips only the same cutscene. Another one in the same town, at another spot or right after a new quest step, plays.

### Other addons

#### Fixed

- Choosing EldoUI for another addon's jobs turns that addon off only when a part EldoUI would replace is switched on in it.
- The bags addon's bag and bank windows follow your layout when you change its skin or switch views.
- Turning another addon off or back on for this character now uses the same character the game's addon list does, so it no longer misses characters that share a first name.

### Options

#### New

- Use Tab and the arrow keys to move through options and setup, change settings, and pick from lists with the keyboard.
- On screens under 1440 pixels tall, the UI scale and Accessibility pages name the smallest text size and offer one button that turns on Large text at the size that brings it to 9 pixels. Undo puts back what you had.

#### Improved

- Color-blind safe colors now follow the game's color-blind mode by default, so turning it on in the game's settings is enough. The Default, High contrast and Large text presets keep following it.
- The /eui help window has a filter box, groups the key and spell commands under Keys and spells and the test commands under Troubleshooting, and shows every command the same way, also in Danish.
- The options window has one name everywhere, and the Keybinds page now sits under Layout and style.
- Reset to defaults on a module page now keeps your window places and your own lists, such as restock items, totem loadouts, reminder spells and your own Fanfare triggers; the built-in Fanfare triggers go back to how they ship.
- A module reset shows up in Recent changes as one step you can undo, and a setting it changes that needs a reload is counted on the Reload UI button.
- Search features waits until you stop typing and keeps the sidebar steady while the same pages match, so typing no longer stutters.
- Option help texts say what a setting does in plain words, without notes about game rules, and a few rows that could never be used are gone.
- Texts across the options and chat messages say "during boss fights" and "version of the game" in place of technical terms.
- Danish tooltips name a setting's default once, and the stripes in search results and Recent changes follow the chosen art style.
- Option names speak to you the same way everywhere ("Alert on your name", "Only your faction"), and the helpers that act for you no longer end every line with where to change them.
- Settings that do nothing until another switch is on are grayed out with the reason, on the Counters, Alerts, Chat input, Mail and Farming pages.
- The same setting has the same name on every page, and help texts no longer show the game's internal setting names.
- The line under the sidebar shows how much time EldoUI takes per frame, read from the game's addon profiler, without turning on script profiling.
- Size, spacing and offset sliders show their unit (px, %), help texts say what a row changes instead of repeating its name, and the Effects styles explain each choice in the dropdown.

#### Fixed

- Undoing a module reset updates which settings still need a reload.
- Undoing a Fanfare reset brings back your previous built-in trigger settings and keeps later trigger edits.
- Mark height on the class resource bar shows a percentage of the bar height.
- Settings that keep their value outside the page, such as the keyboard layout on the Keybinds page, show the saved value and can be undone from Recent changes.

### Performance

#### Improved

- Moving glows use less processing on high-refresh screens while keeping their speed, color and reduced-motion behavior.
- Changing gear with My Adventure open works out the where-next list once instead of twice.
- The gathering pins rest while the world map is closed, and the threat display and combo points on nameplates only listen to the units they show.
- The enemy list, chat bubbles, reputation bar, Edit Mode dimming and Streamer mode skip work that changes nothing on screen.
- The weapon enchant timer updates once a second until its last minute, and not at all when the game's own enchant icons draw the time. The crosshair's range tint pauses while the crosshair is hidden.
- The ready check report follows group auras only while it is open, and guild crafters, chat and Appearances do less work on busy events.
- Nameplates coming into view in busy places reuse their aura icons without checking every aura setting again, and health-colored texts no longer make new data on every health change.
- Zooming the world map keeps the travel, map note and gathering pins in place without building them again, so zooming a continent no longer stutters.

#### Fixed

- Cooldown rows, tracking bars, aura groups, the class bar and the shaman cooldowns reuse their aura frames when they rebuild, so memory no longer grows with each level-up, gear swap or setting change.

### Saved settings

#### Improved

- Player Notes keeps the 300 newest players you only grouped with, so the saved file no longer grows with every group. Players with a note or a mark are always kept.

#### Fixed

- Forget on a character now also removes its run history (after keeping one backup of it), its setup backup, bar snapshots, reminded quests, gather counts, quest tracker state and its bank marks and groups in every profile.
- Journals kept for another character no longer pile up in your saved file: each is stored packed, only the newest ten stay, and the Saved data page can remove one or give an older copy of your own journal back to this character.

### Localization

#### Improved

- The Danish setup, Other addons and action bar texts read as natural Danish, with one word for each idea, and Danish chat lines after selling, buying or saving read the same way throughout.
- With EldoUI in Danish, short numbers and slider values use a decimal comma, such as 1,2k and 0,40.

#### Fixed

- The fishing and farming bars, the ping feed, the waypoint arrow and coordinates and the camp panel show their names in Danish in move mode.
- Dialog buttons and other words the game also uses (Yes, Cancel, OK, Bank, Dead) now follow EldoUI's language, so a Danish dialog has Danish buttons.
- The bag search help, the guide window's check-off tips and the Journal river's marker names show in Danish.

### General

#### New

- Dungeon entry notices in Scholomance and Stratholme link your Argent Dawn trinket when you carry it, have none equipped and are below Exalted.
- Flight Games adds Gnome Dash, with ten courses, coins, checkpoints, and a gnome who grows into a dwarf.
- Open or close Flight Games with /eui fg.

#### Improved

- Disable screen effects also suppresses drunken haze, with a separate choice to keep the game's glow setting.
- Error details show saved local variables below the stack when they are available.
- Snake has a WoW snake and a connected body that grows with every meal.
- Flight Games describes its game types, pace and flight countdown more clearly, with improved Danish game names.
- Fill in DELETE automatically is off until you turn it on, picking a look no longer turns it on, and it is listed with the other helpers that act for you.
- Flight Games is on for everyone: the Games box shows on your next flight path. If you switched it off, it stays off, and the Modules page turns it on or off at any time.

#### Fixed

- The AFK screen waits while an NPC interaction, cinematic, movie, or barber shop is open.
- Your name updates immediately when you change My Secondary Name in the game's settings.
- Player names in loot windows, raid loot lists, reminders and combat notices use a font that can show more alphabets.
- In the error log, an entry from an earlier day shows its date instead of only a time, and the copied details use EldoUI's date format.
- The error log keeps older dates readable when you change language or text size.
- Quickdraw spell entries use the highest rank you know and update when you learn a new rank.
- Board games use your faction's names, banners and colors.
- The character in Candle Mine faces the direction it runs.
- Fishing's Louder splash never turns your master or effects volume down, and Quieter music never turns up music you keep silent.
- In the error log, an error that repeats every frame no longer crowds out new errors, its count is exact, and the open log window stays readable and selectable while it repeats.
- Bringing an older profile up to date no longer stops with an error when its durability reminder was left at the default.

### Classes

#### New

- **Druid:** Druids can give Prowl its own action-bar page while keeping their normal cat-form page.
- **Hunter:** Hunters can mark the food their current pet can eat in their bags.

#### Improved

- **Mage:** How to play lists Teleport: Dalaran in the travel menu with the other teleports.

#### Fixed

- **Paladin:** Gear comparisons use ranged hit for Judgement.
- **Priest:** The Class Bar offers Shadow Word: Death and your race's priest cooldowns, with a separate switch for each spell.
- **Rogue:** The class bar shows the off-hand poison icon again while you wield an off-hand weapon.
- **Shaman:** Gear comparisons use Stormstrike's eight-second cooldown.
