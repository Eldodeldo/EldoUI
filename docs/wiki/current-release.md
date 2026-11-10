# Current release

<!-- eldoui:release-docs 0.7.2000 -->

EldoUI **0.7.2000**, 2026-11-10.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.2000) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.2000/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Highlights

- The dungeon map shows the game's minimap large in Live, and WoW: Forever's own dungeons open it with their boss list.
- All nine WoW: Forever dungeons have their own Journal pages, and quests say where they sit in their chain.
- A class bar for every class but the shaman keeps your buffs, auras and key cooldowns in view.
- Spell cues flash the buttons of a spell the game lights up, with an optional sound.
- A layer chip on the minimap shows your layer and hops you to another with a click.
- New class reminders for warlocks, rogues, priests, warriors and druids, and a Pet abilities tab for hunters.
- Player nameplates wear their class color, so players stand out from friendly NPCs.
- Modern Center, Portrait Staggered, Nameplate Focus and Twin Orbs have new versions in the setup.

### Setup and profiles

#### Fixed

- A new character that shares its first name with one of your older characters now starts with its own setup and the class default profile, instead of taking the older character's profile and options. Settings you forget for a character no longer come back at its next login.

### Layouts and move mode

#### Improved

- Window moving has its own Move windows page with a check box per window, Lock windows and a key to drag (Ctrl, Shift, Alt or two keys), so a slipped click on a quest's Accept button never moves the window. Move mode needs no key.
- Modern Center, Portrait Staggered and Nameplate Focus have new versions in the setup: the zone toast gets a clear spot under the ready check and Party Quests opens clear of the quest tracker. Profiles on the earlier versions keep their positions.
- Twin Orbs has a new version in the setup with the bag bar a little lower, clear of the statue beside the power orb. Profiles on the earlier version keep their positions.

#### Fixed

- In EldoUI Center, Compact HUD, Widescreen Edges, Open Center, Close Combat and Twin Orbs the Enemy Spotter list grows upward from just above the raid frames, so a long list no longer covers them.
- On 16:10 screens, Blizzard Bottom Block puts the micro menu and the bags in a row in the bottom-right corner, so they no longer sit on action bar 4 or the stance bar. With large action bar buttons the Battle.net toasts move above the chat there.
- In Vanilla Original the loot roll bars no longer reach under the talking head, and in the new Modern Center the talking head stays clear of the loot rolls and the waypoint arrow, also with a large minimap.
- In Twin Orbs the shopping list sits below the boss mod's info box, as in the other layouts, instead of reaching under it.
- The Feed Pet button keeps clear of the pet, player and focus frames in every layout: with a unit frame style that makes them larger (or larger action bar buttons in Open Center), it moves to a free spot next to them.
- In Modern Center the right chat panel sits a little lower, clear of the target of target and the quest timer.
- On 16:10 screens the boss mod's info box no longer covers the ping feed in Blizzard Bottom Block and Portrait Staggered, and in Portrait Staggered the right chat panel keeps clear of the target of target.
- On 16:10 screens Portrait Staggered's extra ability button keeps clear of action bar 4 and the bag bar, and its boss mod info box clear of the swing timers.
- On 16:10 screens Twin Orbs' boss mod info box keeps clear of the encounter bar, and Modern Center's boss frames and popup dialogs of the raid warnings and the talking head.
- In Vanilla Original, unit frame styles with a wider target frame put the popup dialogs below the talking head instead of under it.

### Unit frames

#### New

- The execute shade can take its range from your own spell: with "Use my execute spell" on, it follows Execute or Hammer of Wrath once you know it, on nameplates, unit and group frames alike.

#### Fixed

- Class resources and the player cast bar set above or below the cooldown manager keep working and keep their place when the cooldown rows cannot be measured.
- In test mode the target of target frame shows a short label when its full title does not fit.
- After a layout or setup is applied, a frame placed above a unit frame with its name on top, such as the pet above the player, keeps its gap above the name.

### Group frames

#### Fixed

- The Ready Check Report counts Nightfin Soup and the stat foods, such as Grilled Squid and Runn Tum Tuber Surprise, as food. Nightfin Soup no longer reads as Mageblood, and a Shadow Protection Potion no longer reads as the priest buff.
- Raid Tools' Ready and Roles dim when the game would ignore you, and a click says that only the leader (or an assist in a raid) can start them.
- The Ready Check Report counts WoW: Forever's Natural flasks and its new elixirs, such as Greater Cleric's Elixir and Greater Mageblood Elixir, instead of reporting a missing flask or elixir.
- With click casting's hover keys on, a party or raid frame that disappears under your mouse (a player leaves, the frames hide) lets go of those keys, so your own key bindings work again instead of casting on that player.
- A click anywhere on a party or raid member's frame targets them, also on the name, the bars, the aura icons and the portrait.
- With click casting on, nameplates that come into view no longer fill the error log with a Lua error each time.
- With the light skin on Blizzard's party and raid frames, a frame whose name the game keeps hidden no longer raises a Lua error; it is left unskinned.

### Nameplates

#### New

- Players stand out in a crowd: their plates wear a border in their class color, and friendly players' bars take their class color too, so they no longer look like friendly NPCs. Pets and minions get a slightly smaller plate. Both are in the Colors and General tabs.

#### Improved

- Quest mobs are light blue and elite mobs aqua, so a hostile quest mob no longer wears a green close to friendly NPCs.

#### Fixed

- Tanks in Defensive Stance, Bear Form or with Righteous Fury get tank threat colors without a group role, and plates and the target frame warn while someone catches up on threat.
- EldoUI plates show the game's soft-target icon again, above the name of the unit you'll interact with, when the game's icon setting for it is on. A new Target option, "Highlight your soft target" (off by default), gives that enemy the mouse-over look.
- In a group, quest progress on a plate shows your own objective, never a party member's.
- A fishing bobber, herb or ore node that gets a plate for its interact icon keeps the game's icon instead of an empty health bar.

### Action bars

#### New

- Spell cues, off until you turn them on: when the game lights up a spell, its buttons flash once, with an optional sound. Your buffs glow on the spells they change, such as Maelstrom Weapon with its stacks on Lightning Bolt, and your own effects on their button while they last.

#### Fixed

- Cast on now shows when your spells cast and gives you the chat command to switch, since the game does not let an addon change that setting.
- Hidden action bars no longer wait on top of an orb's statue when you drag the power orb toward the lower-right corner.
- A bar set to show on mouse-over stays visible while your mouse is on a flyout you opened from one of its buttons, in combat too, and fades as usual once the flyout closes.

### Talents and spells

#### Fixed

- The level-up card and the Journal's class quest list show the class quest for your own race, with the map pin on the start nearest you, and now include WoW: Forever's own class quests, such as Cat Form, Summon Incubus and the quests for the new race and class pairs.
- The Trainer pin on the level-up card finds WoW: Forever's own class trainers, such as the Ironforge shaman trainer, once you have opened them, and points mages to a portal trainer for their portal ranks. Trainers in Exodar and Silvermoon are gone from the weapon trainer list.
- The trainer list and the level-up card no longer offer spells the game removed: Frost Blast, Binding Heal, Lava Burst and the last Primal Bite rank. Mutilate's ranks follow the talent, and Primal Bite's ranks show at 50 and 60.

### Auras and cooldowns

#### New

- New ready-made aura groups: Sunder Armor, Rend and Demoralizing Shout for warriors, your seal for paladins, and Flame Shock for shamans.

#### Fixed

- The private aura slots next to your debuffs come back on their own after a layout that could not be measured, without a reload.

### Combat

#### New

- A class bar for every class but the shaman, off until you turn it on: the buffs, auras, armors, aspects or poisons you keep up (live in combat, faded while missing), your key cooldowns and the reagents or ammo you carry. Each icon has its own switch.

#### Improved

- Combat Text has its own move mode. Move areas unlocks only the scroll areas, plays sample lines in each one's own look, marks the edge where new lines start, and lets you resize a box from its corner.
- In that move mode, areas that are off show dimmed so you can place them first, and right-click turns one on or off. Move this area unlocks just the area you are editing, and Reset every area puts them all back on your layout.
- The Danger Alerts description now says plainly what the alarms warn about.

#### Fixed

- The Consumable Bar puts conjured food and water first on every game language, not only English.
- Showing Blizzard's damage meter or loss of control alert again gives back your own game setting once, and a later change in the game's options stays.
- The Consumable Bar keeps WoW: Forever's buff foods and Nutritious drinks out of the automatic pick, and battleground and Darkspear Islands rations show on both the Food and Drink buttons.
- The Minimal and Blizzard-like combat text styles no longer move the Incoming text to the bottom of its area, below where your layout puts it. A profile that already used one of them gets its Incoming text back at the top of the area.
- The "Attacked while AFK" alarm also sounds when the game briefly hides whether you are away, using the last state it showed, and aura alarms set up during a fight or a boss encounter (after a reload) start once it ends instead of staying off.
- After a group fight the combat timer you keep on screen switches to the fight's full length as soon as the game shows it, so it matches the Info Bar's combat time instead of stopping at your own.
- A damage meter row that first appears during combat no longer causes a secret-value error; its border shows once combat ends.

### Info Bar

#### New

- Arcane, Fire, Frost, Nature and Shadow resistance can each go on the bar, with what your gear adds and your average reduction against your level and a boss three levels higher.

#### Fixed

- In dungeons and raids, where the game hides /roll results from addons, the roll window and the Rolls block say so instead of staying empty.
- Clicking the Honor bar or the Honor block opens the PvP tab of the character window, and the Honor bar fills with your honor points toward the most you can hold.
- Hovering the Guild block during a boss fight, a key or a PvP match no longer causes an "Interface action failed" error. The guild message of the day is left out of the tooltip until chat opens again.
- Warriors and rogues with a bow, gun or crossbow see their ammo count in the Ammo block and on the quiver too, and ammo that doesn't fit the weapon shows in the warning color. The low ammo warning can be turned on for them as well.
- Clicking a block that opens the character window (Durability, Item level, stats and the like) no longer raises a Lua error in combat. In combat the block now says "Not in combat.", as other blocks that wait for the end of a fight do.

### Chat

#### Improved

- A new whisper opens its messenger window straight away when you are out of combat, so it is no longer missed in the dock. A whisper that arrives in a fight waits in the dock and its window opens when the fight ends. "Show in the dock" and the Quiet style keep the old way.

#### Fixed

- For characters with a surname, player notes match the same player's chat lines, chat levels and guild mutes find the sender, and Streamer Mode hides your own name in your chat lines.
- Saved chat and message history no longer show a Battle.net friend's name as stray codes or a wrong name after you log in again; conversations are kept under the friend's BattleTag.

### Tooltips

#### Improved

- Item tooltips show the auction price for everything you have seen at the auction house, also from searches in the game's own Buy tab and its buy screen, with how many days ago it was seen. The Shopping List tab's Full scan button fills in the whole auction house in one go.

#### Fixed

- Holding or releasing Shift over a nameplate, another unit the game keeps hidden, or a tooltip with hidden text colors no longer raises a Lua error in the game's tooltip.

### Bags and loot

#### New

- Humar the Pridelord, Swiftmane and Takk the Leaper in The Barrens list the WoW: Forever set Blessing of Kalimdor first on the World page, with how many pieces you have.
- Catalog > PvP lists what WoW: Forever's rank vendors sell: the Premier armor and weapons, the Emboldened seals, the new tabards and insignia, for your side.
- Item scores can weight Fire, Nature, Frost, Shadow and Arcane resistance, so resistance gear shows its gain on a scale made for a raid that needs it. Scale strings keep these weights.

#### Improved

- The Loot Guide's World events follow the game's calendar in every client language, show when each event next starts, list the fishing contest's coin and prizes, and leave out the events WoW: Forever does not run.
- The Loot Guide knows the short forms for WoW: Forever's dungeons and raids (hot, rol, bd, hs and more), "ruins" opens Ruins of Lordaeron, and a short form two instances share, such as st or dm, lists both.
- On an account without an authenticator, the bag window's footer shows the backpack's 4 locked slots; hover it to see how to unlock them.
- The Account bank option and the guild bank choices (window, bag tooltip count, opening bags with the guild bank, repairing from it) show only when the game has that bank, so no option sits there doing nothing.

#### Fixed

- The bank's buy-a-tab button waits for the end of a fight before it moves, and then follows the bank bar.
- A bank window that closes as the bank sends its last update no longer keeps its bank-only buttons.
- Prices from a neutral auction house (Booty Bay, Gadgetzan, Everlook) are kept apart from your faction's, so a visit there no longer changes your prices at home. Quick Sell shows what you receive after the house's cut, and warns when that is below the vendor price.
- The Loot Guide shows WoW: Forever's own quality, item level, required level, bind, set, slot and weapon speed for over 900 items that changed since Classic, and leaves out six items the game does not have.
- An item whose stats changed on WoW: Forever is rated on its real stats once the game has loaded it, never on its old ones.
- Weapon and defense skill-ups gained in dungeons and raids now show their toast and combat text line too.
- Catalog > PvP has a Darkspear Islands group with the Darkspear Raiders and Theramore Expeditionary Force rewards for your side and the standing each needs, and the wallet counts Darkspear Islands Marks of Honor.
- Free bag slots set back to Game setting gives back your own choice, and a later change in the game's options stays.
- The gear simulator plays Enchant Weapon - Lifestealing: its Shadow damage counts toward the result, so a Lifestealing weapon no longer scores as if it were bare.
- The Loot Guide's map buttons open the world map the way the game does, so quest pins and their Share button keep working afterwards, and while the game holds the map back they ask you to open it with M.
- Catalog > PvP reads your rank from the season track, so rewards you have reached no longer show in red, and the rank each reward needs is the one the game reports.
- The Loot Guide's gear simulator follows WoW: Forever's combat rules: damage over time and channeled spells can crit, expertise lowers the target's dodge, spell hit reaches 100 %, druid forms use the Feral Combat skill, and spells count spell power as the game's own data says.
- Best in Slot plans and upgrade arrows respect the rings and trinkets the game lets you wear only one of at a time, such as the Watchers' signets and the engineering combat trinkets.
- The Loot Guide marks Molten Core, Blackwing Lair, Zul'Gurub, both Ahn'Qiraj raids, Naxxramas and the world bosses as not in WoW: Forever yet, and stops suggesting them or planning Best in Slot with their loot.
- The Loot Guide lists Barrow Deeps and Hyjal Summit as announced raids.
- The Alts window's First Aid column shows each character's skill, and the Info Bar's profession tooltip and the loot feed's skill-up icons no longer miss a profession that follows an empty slot.
- Every empty slot in the bag window has the same dark look again; the game's own brown empty-slot picture no longer shows on some of them.
- The first bag open of a session in combat, or of a bigger bag you just equipped, shows every slot at once instead of an empty window until the fight ends.
- A group roll whose item takes a while to load still gets its roll bar as soon as the item is there, with the time that is left, instead of being dropped after a few seconds.
- Faster auto loot and the loot window's Loot all button take one item at a time in quick succession instead of a whole pile at once, never loot the same corpse twice, and stand back while the group uses master loot.
- Right-clicking an item in the EldoUI bank window now takes it out to your bags.
- When several items go up for roll at once, every roll now gets its bar in EldoUI's roll bars, also when the game is still loading an item's details. That bar shows as soon as they arrive.

### Journal

#### New

- All nine WoW: Forever dungeons are in the Journal's overview with their level range and zone, each with its own page. A boss is added there the first time you defeat it, with the items you see it drop.

#### Fixed

- A Skyborne character sees its own side's quests and items as meant for it, instead of almost every quest marked as not for you.
- A WoW: Forever class quest whose spell the game has not named yet shows as Class quest in its list, never as an internal code.
- The Loot Guide follows WoW: Forever's own schedule instead of Classic phases: Onyxia's Lair, Barrow Deeps and Hyjal Summit show the day they open, their loot is marked until then, and Best in Slot can plan with or without the December raids.
- Kormok in Scholomance, Jarien and Sothos in Stratholme and Mor Grayhoof in Upper Blackrock Spire now have their boss cards and drop lists, like the other summoned Dungeon Set 2 bosses.
- The Shaper's Terrace names its zone, Un'Goro Crater, and Krol'dok Stronghold names Riverglades in your game language.
- Dungeon, raid and battleground runs show again in My Adventure and in your alts' run lists and counts, for characters with a surname too, and forgetting a character removes its runs.
- Places you have been to are no longer a "First visit" again. Characters that share a first name set each other's journal aside in earlier versions; each character now gets its own journal back, with every place it has visited.
- The Fellowship list opens without an error when someone you know only from your player notes has no known level.

### Leveling and quests

#### New

- WoW: Forever's own quest chains that the game lists, such as Toxic Soil in Westfall, show every step in order in the Journal.
- The quest window, the quest log and the dialog view say where a quest sits in its chain, such as "Part 2 of 5, next: The Defias Brotherhood (level 18)". Hover it for the whole chain, click it to open the quest in your journal.

#### Improved

- Eldostar checks off flight, vendor, class trainer and talk goals by itself when you land, open the merchant, close your class trainer or talk to the right NPC, so a town no longer needs a click per goal.
- An Eldostar goal to complete a quest lists the quest's objectives with their counts under it while the quest is in your log, the finished ones dimmed, and the compact view shows the first one still open.

#### Fixed

- Eldostar's accept and turn-in steps point at the quest giver or ender for every quest the Journal knows, and at the place you met them yourself when you have.
- The XP bar tooltip, the Info Bar's rate blocks and My Adventure now show the same XP per hour and time to level, counted from one session that goes on over a reload and with the Info Bar off. The tooltips say whether the rate reads the last hour or this session.
- Rested XP estimates follow the Legacy talent Well Rested. Each character learns its rested rate and cap from what the game gives it while away, so the overview, Full in and the rested planner stop calling a bar full too early.
- The mount guides list WoW: Forever's new mount colors and say which riding each racial mount needs, so you no longer buy a mount your race cannot ride yet.
- The Onyxia guide step names the Drakefire Amulet as the attunement for both factions, and says each raider needs their own.
- The Agenda shows each holiday once, not once a day and once per character, and reminds you of it only once.
- Before you hand in a quest whose work is not done, Eldostar says its objectives are still open, lists them and points you to the work instead of the quest giver; its goals along the way stay listed until the work is done.
- Eldostar's waypoint goes to the nearest camp or quest giver on the step's zone instead of the largest camp anywhere, and with several kill or collect goals it points at the nearest one without jumping around in a fight.
- The quest addon's tracker no longer causes a blocked-action error when it turns up during combat; it moves onto the Quest Tracker spot when combat ends.
- A guide step no longer waits forever to hand in a quest the guide only picks up when you happen to get it, such as one that starts from a rare drop; the goal stays visible, dimmed, in case you have it.
- The NPC dialog view shows quest levels in their difficulty colors and marks quests new in WoW: Forever, like the game's quest giver window. Reward choices show their sell value when "Sell value on quest rewards" is on, with the most valuable one highlighted.
- Turning in quests automatically never pays for a quest that costs gold, and leaves repeatable quests such as reputation hand-ins to you, so a whole stack is never handed in at once. "Leave repeatable quests to me" turns the second part off.
- The Salt Shaker's three-day cooldown is now saved like the recipe cooldowns, so it shows in the Agenda, the Overview's cooldown column, the cooldown reminders and the Profession Planner.

### Map and minimap

#### New

- Live on the dungeon map shows the game's minimap large, with your arrow, your group and the rooms; on a wide map it sits beside the painted floor.
- WoW: Forever's own dungeons open the dungeon map in Live with their boss list, checked off as you kill them.
- A layer chip on the minimap shows which layer you are on. Click it to hop to another layer through players who offer help, in your guild or in the layer network that the layer addon's players share too. Every invite, accept and leave is your own click.

#### Improved

- Inside a dungeon, the world map now shows the game's painted map of the floor, with the bosses as skulls and a boss list beside it that checks off the ones killed in your lockout.
- Packs, patrols and routes no longer cover the dungeon map. Turn on Packs and route to see them there; the Dungeons window always shows them.
- On a dungeon's painted map, packs, bosses and route marks sit where they stand in the dungeon on every floor, and each floor is named in the floor list.

#### Fixed

- Transport Maps show WoW: Forever's own routes: the Stormwind Harbor ship to Auberdine, the goblin ship from Steamwheedle Port to Powderfuse Port, the Feathermoon ferry and the Zephras Isle skyboats. The Menethil ship now runs its loop through Southshore.
- The world map shows the level range of the zone you look at again, and the map, Zone Info and My Adventure always give the same range.
- The Deeprun Tram pins sit on the tram entrances in Stormwind and Ironforge.
- Layer hop waits for the game's own layer-move countdown and shows it on the layer chip, shows "L ?" until the new layer is read, and says when the game limits how often you can change layer.
- Minimap Rotate set back to Game setting gives back your own choice, and a later change in the game's options stays.
- Opening the world map with unexplored areas shown, or with dungeon entrances drawn, no longer raises a Lua error.
- Flight times count the Frequent Flier talent: each route shows its time at your own flight speed, and a flight with the talent no longer throws off the time kept for that route.
- Zul'Farrak, Zul'Gurub and the Ruins of Ahn'Qiraj have their painted dungeon map, and Uldaman shows all three of its floors.
- The flight timer remembers each route's time again: a route you have flown before shows the time left instead of "learning".
- Your world map coordinates no longer show twice when the game's own coordinate setting is on: each position EldoUI shows hides the game's matching one, and the game's come back when you turn EldoUI's off. The gamepad crosshair position still shows.
- Ctrl+right-click (waypoint) and Alt+right-click (map note) on the world map no longer zoom the map out, so the new pin stays in view.
- Opening the world map or the quest log no longer logs "EldoUI tried to call the protected function" for map pins or the Share button. The Info Bar's map and quest blocks and the flight view's map button let the game open these windows, in combat too.

### Windows and skins

#### Fixed

- Changing the style, skin or palette no longer stops with an error part way, leaving some boxes in the old colors.
- A window you drag by one of its side panels stops following the mouse when you let go, even if that panel closed during the drag.
- Sell values on quest rewards sit on their own line at the bottom of each reward button, below the item name, instead of spilling over the icon and the stack count.

### Notifications

#### New

- The level-up toast lists the spells and new ranks your class trainer teaches from your new level; a click opens the spells to train. The Journal's chapter card shows them too when it takes the level-up. Turn it off with "New spells on level up" in the alert lane settings.
- Rare Alerts treat a set piece you don't have yet like a missing mount, pet or toy: the card shows it and plays the notable sound.

#### Fixed

- The Battle.net toast goes back to its own spot each time a GM ticket box closes, not only the first time.
- Aura alarms that wait for a boss fight or a match to end no longer switch on as the next one starts, so they are not lost for the session.
- Rare Alerts no longer raise a world boss card when you target or pass a friendly city leader such as Thrall or Bolvar Fordragon.
- Fanfare's big text and icon stay off the screen during a boss encounter, where they covered the boss mod's info box, and a pull clears them. The sound and the screen flash still play.

### Other addons

#### Fixed

- Switching an addon's layout spot off and on again in one fight leaves its frame placed after combat.
- A leveling guide placed near the top of the screen opens downward: its current step card sits under the guide instead of above it. A new setting on the guide's integration tab turns this off.
- The meter reset command says so when your damage meter addon cleared every fight it stored as well, since that addon clears its own history along with the game's meter.
- Damage meter windows snapped into a group stay together: moving or resizing the group moves every window's spot with it, also when you do it in combat, and a reload keeps them where you left them.

### Options

#### Improved

- New Reduce motion switch on the Accessibility page, shared with Animations on the General page. It now also holds glows, the lit dungeon map pin, the bag item flash and combat text shakes still; highlights stay as steady borders.
- A slider follows the mouse without lag while you drag it, and its live preview redraws at most once per frame.
- The Style presets page lists the parts of the UI, and each opens to its styles with a click; the Move windows page folds each group of windows.
- Option texts, tooltips and the setup use the same US English words everywhere: check boxes are checked and unchecked.

#### Fixed

- The camera options leave protected game settings alone instead of trying to change them after combat, which the game refuses.
- The sidebar scrolls to a whole row when it follows the page you open, so a group heading at its top is never cut in half.

### Performance

#### Improved

- Nameplates listen only for what they show: with the power bar, cast bar or absorb shield off, the plates no longer wake for those updates, friendly plates skip threat updates, and another group member's threat change no longer recolors every plate.
- A nameplate updates its health and absorb shield once per frame however many changes arrive together, and the execute and low-health shades do less work on each health change.
- While EldoUI draws every kind of nameplate, Blizzard's own plate under each one stops updating in the background, so each plate's work is done once. Leaving a kind to Blizzard's plates asks for a reload.
- The target of target, focus target, pet, party pet and party target frames listen only to their own unit, so another player or a mob changing its target or pet no longer redraws them.
- Class resources listen only to your own character: another player's or a nameplate's health, power and casts no longer wake them, one power change is one refresh, and the combo point colors are set only when they change.
- Heal prediction and absorb shields on unit and group frames update without making new memory on every health change, which keeps big raid fights smoother.
- Group frames listen only for the parts they show: without a power bar, portrait or threat border a raid no longer wakes for every member's mana tick or model change, and a healer-only power bar follows role changes.
- When a raid forms, a battleground fills or members swap groups, group and unit frames refresh once for the whole burst instead of once per change.
- Info Bar blocks that update often (frame rate, latency, coordinates, timers) only redraw when their text changes, and a digit changing no longer shifts the blocks next to them.
- Selling, looting or moving an item with the bags open no longer rates every item in your bags again for the upgrade arrows; only a change of gear, level, talents or scales does.
- The bag window no longer redraws in full after every sale, loot, XP tick or quest update; only views of another character, all characters or the guild follow their saved records.
- The saved undo history of layout switches keeps to a quarter of its old room, so the saved settings file stays smaller and loads faster.
- Instant Messages reuses the window of a closed conversation for the next one, and the dock makes only as many buttons as it shows, so a busy whisper session no longer piles up windows.
- Upgrade ratings keep a bounded memory in long sessions of Loot Guide lists, auction searches and item tooltips.
- Logging in and reloading the interface is quicker: the Loot Guide's translations are read only on a game client in their own language.
- The DPS and HPS blocks on the Info Bar read Blizzard's damage meter only when it has new numbers, and once a second in combat, instead of every second all evening.
- Loading screens are lighter on the action bars: only a login or reload rebuilds every bar, bars 6 to 8 are made only once you turn them on, cooldown updates skip empty and hidden buttons, and another player's pet no longer wakes the pet bar or the experience bar.
- After a bag change only the bags that changed are read again for your saved inventory and item counts, so looting and selling stay light with large bags.
- The character window, the away screen, Hardcore and spell cues listen only to your own name, flag, faction and pet changes, so they stay quiet while a raid changes around you.
- Health, power and name texts on unit frames, group frames and nameplates wake only for their own unit, so a raid's health changes no longer touch every text.
- Item tooltips reuse the character list and the counts of who holds the item between redraws, and stop reading each tooltip line when no line-hiding option is on.
- Saved auction prices for your other realms and factions are kept packed, so logging in and reloading read them much faster. They unpack the first time a character there needs them, and the Auction page's Data section shows how much the saved prices take.
- The dialog view rebuilds a quest page once when its reward items come in, and the NPC model no longer reloads or flickers when the page changes for the same NPC.
- Minimap pins for gathering nodes, map notes and waypoints do no work while you stand still and are redrawn only when they show something else. Map positions are shared and worked out without asking the game each time.
- Boss timers that start together at a pull, battleground score updates and timer bars now share one redraw per frame, the chat filters do less work per line, and a repeated line in a busy channel stays hidden instead of slipping through after many other lines.
- The bag window answers faster: typing a search or hovering a bag button only fades the slots, a sale or a new stack count repaints just that slot, and bank deposits, sorting and quest changes redraw once per burst.
- The cooldown viewer skin does less work when buff icons come and go in combat: one refresh per frame, and each icon keeps its skin and keybind text until something about it changes.
- Party and raid frames follow the game's own range updates for the out-of-range fade, instead of checking every member twice a second.
- An error that repeats every frame no longer slows the game: the error log counts a repeat without reading it again, keeps one entry when only a memory address in the message changes, and logs at most ten a second.

### Saved settings

#### Fixed

- Put back on the Saved data page is refused during combat, like Undo restore and Restore backup, so nothing reloads mid-fight.
- When the game lacks the memory to load EldoUI's saved settings, EldoUI says so in chat and keeps the setup closed instead of starting over like a new install.
- After the update, each character keeps its bar snapshots, reminded quests, gather counts, farming sessions, its groups and bank mark in the Characters window, and stays hidden there if you hid it. Before, these were left behind under the character's old name.
- Two characters with the same first name on one realm no longer share EldoUI data such as their level, gold, bags and dungeon log. Each keeps its own under its full name, and the data saved so far stays with the character it belongs to.
- The gold your other characters see for a character no longer drops to 0 after a logout or a loading screen.

### General

#### Improved

- A burst of blocked actions on a row of numbered frames, such as the twelve buttons of one action bar, is one entry in the error log instead of one per button, which keeps your saved settings smaller.
- An error that comes back after an update shows where it happens now in the error log and in a copied report, with the version and place of its latest session.

#### Fixed

- Fishing's Same key loots the bobber tells you when the game's soft interact is off for mouse and keyboard, and gives you the chat command to turn it on.
- A word that many settings share no longer fills the whole Finder list, so the item, mount or toy with that name still shows.
- A copied error report shows the local variables of the function that raised the error, and a blocked action no longer lists unrelated ones.

### Classes

#### New

- **Druid:** With the tank role, a reminder to shift into Bear Form, or Dire Bear Form once you know it.
- **Hunter:** A Pet abilities tab beside the Training tab lists every pet ability rank with its pet level and training points and what your pet can learn now. For the rest it names the pet trainer or the beasts to tame, with a map pin on the nearest one.
- **Hunter:** The Pet abilities tab shows how often your pet attacks, since a tamed beast keeps its own attack speed.
- **Priest:** Optional reminders for Fear Ward, Shadowguard and Touch of Weakness, shown once you know the spell.
- **Rogue:** Right-click a poison reminder to pick a poison for that weapon; a click then puts the highest rank you carry on it. With none in your bags the icon dims and says which poison is missing.
- **Warlock:** Reminders to make your Healthstone, Soulstone and the Spellstone or Firestone you pick, one click each, with your Soul Shard count. In dungeons and raids a Soulstone reminder names your group's healer and a click puts the stone on them.
- **Warrior:** With the tank role, reminders for Defensive Stance (a click takes it) and for a missing shield.

#### Improved

- **Warrior:** Battle Shout counts as a group buff: the reminder counts party members without it, and the group frames can mark them.

#### Fixed

- **Druid:** The key map's Bear Form movement key holds WoW: Forever's Feral Charge talent instead of the old one.
- **Druid:** The trainer list and the level-up card show Ferocious Bite's new first rank at 24, Lacerate's second rank at 34 and Poised at 32.
- **Druid:** The resurrection entry in Quickdraw uses Revive, so Rebirth keeps its long cooldown for combat.
- **Hunter:** The key map treats Aimed Shot as the trainer spell it is now, not as a talent.
- **Hunter:** The trainer list and the level-up card show Enchanted Flare at 32.
- **Hunter:** The gear simulator follows WoW: Forever's Aimed Shot, Multi-Shot and Barrage, and counts Lone Wolf, Careful Aim, Rapid Killing and Focused Fire.
- **Hunter:** The Trueshot Aura reminder works from the first rank at level 32, and the higher ranks of Aspect of the Beast count for the rank check.
- **Mage:** The trainer list, the level-up card and Mage Travel show Teleport: Dalaran at 50.
- **Paladin:** The trainer list and the level-up card show Hammer of the Righteous at 40.
- **Paladin:** The Blessing Plan, reminders, ready report and trainer list no longer offer Blessing of Light and Blessing of Salvation, which are gone from the game. Holy Shield's ranks show at 40, 50 and 60, including the new fourth rank.
- **Paladin:** A blessing plan from the group changes the other paladins' rows only when it comes from the group's leader or a raid assistant; any other paladin can set only their own row.
- **Paladin:** Seal of Fury and the first rank of Seal of Righteousness count as seals for the seal reminder.
- **Priest:** The key map treats Divine Spirit as the trainer spell it is now, and leaves the healer key Lightwell had free for your own pick, since Lightwell can no longer be learned.
- **Priest:** The key map now places every race's priest spell: Divine Grace, Contingency Plan and Dark Sacrifice share the movement key with Desperate Prayer, and Chastise and Confounding Flash come before Devouring Plague on the Second stop key.
- **Rogue:** The trainer list and the level-up card show Shank at 24 and 44, the higher Death Mark ranks at 48, 56 and 60, and Poised at 18.
- **Rogue:** The Ambush cue for Cutthroat is gone: the game no longer gives that buff.
- **Shaman:** The Lava Burst ready icon and its spell cue are gone with the spell, and the Elemental capstone is called Lightning Mastery.
- **Shaman:** Clicking the weapon imbue reminder casts the highest rank you know instead of the first one.
- **Warlock:** The demon reminder counts the Incubus as your demon and has its own Incubus setting. Texts use the game's names Bane of Agony and Bane of Doom.
- **Warrior:** The key map places Victory Rush on the self heal key, Tactical Mastery among the passives and Heroic Strike's top rank from its manual, and shows Charge in Defensive Stance once you have Vanguard.
