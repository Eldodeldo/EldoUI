# Modules

Everything in EldoUI is a module you can switch on and off: 96 modules in all, listed below by area. Each one has its own page in the config window (`/eui`, then its name in the sidebar).

- `/eui modules` lists every module and whether it is on.
- `/eui <name> on`, `off` or `toggle` switches one. The name is the word in the table below, the module's name as the config window shows it (`/eui party and raid off`) or a unique start of it (`/eui na off` switches Nameplates off), ignoring case and spaces. `/eui <name>` alone opens its settings.
- A module stays off while an addon that does the same job is loaded (for example Bags while Bagnon or Baganator is loaded), so two addons never draw the same thing.
- "Default" is the state in a new EldoUI profile; a module marked Off waits until you turn it on. The setup's Modules step, a preset pack or the UI amount can change it, and anything you switch off leaves Blizzard's own version in place. Party Quests starts on and shares your quest progress with group members who run EldoUI, as addon messages only, never chat; never in battlegrounds or arenas, and not in raids unless you allow it.

Each module name links to its section in the showcase.

## Interface

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Info Bar](../showcase/features/interface.md#info-bar) | Full-width bars and your own datatext panels with clock, gold, durability, stats and more. | `infobar` | On |
| [Minimap](../showcase/features/interface.md#minimap) | Square or round minimap with zone, coordinates, clock, button placement and an addon button bin. | `minimap` | On |
| [Tooltip](../showcase/features/interface.md#tooltip) | Clean tooltips in the game's own style with quality and class borders, a tidy info area and a movable anchor. | `tooltip` | On |
| [Maps](../showcase/features/interface.md#maps) | World map, quest log, flight map, battlefield map and UI widgets: skin, position, scale, coordinates and fading. | `maps` | On |
| [Quest Tracker](../showcase/features/interface.md#quest-tracker) | Blizzard's quest and objective tracker: EldoUI look, mover, height, font, fade in combat and Questie support. | `objectivetracker` | On |
| [XP and Reputation Bars](../showcase/features/interface.md#xp-and-reputation-bars) | Experience, rested XP, reputation, honor and pet experience bars in one movable stack. | `statusbars` | On |
| [Micro Menu and Bag Bar](../showcase/features/interface.md#micro-menu-and-bag-bar) | Move, resize and restyle Blizzard's micro menu and bag bar, or fold them into the Info Bar and bag window. | `micromenu` | On |
| [Alerts and Banners](../showcase/features/interface.md#alerts-and-banners) | Toasts, banners, talking head, raid warnings, red error text, zone text, ready checks and cutscenes. | `notifications` | On |
| [Loot](../showcase/features/interface.md#loot) | Loot window, group roll bars, loot history and loot toasts in the EldoUI look. | `loot` | On |
| [Character Panel](../showcase/features/interface.md#character-panel) | The character window, its slots and side panels in the EldoUI look. | `character` | On |
| [Friends and Social](../showcase/features/interface.md#friends-and-social) | Friends, guild, calendar, group finder and PvP windows in the EldoUI look, with class colors, a friends search and movable windows. | `social` | On |
| [NPC Windows](../showcase/features/interface.md#npc-windows) | Quest, gossip and other NPC dialogs, the pet stable and the barber shop in the EldoUI look. | `npcwindows` | On |
| [Window Skins](../showcase/features/interface.md#window-skins) | Spellbook, talents, professions, trainer, Legacy, collections, socketing, dressing room, and inspect windows in the EldoUI look. | `skins` | On |
| [System Windows](../showcase/features/interface.md#system-windows) | Game menu, Settings, AddOn list, keybinds, macros and pop-ups in the EldoUI look, with a few safe extras. | `systemui` | On |
| [Edit Mode](../showcase/features/interface.md#edit-mode) | EldoUI's frames inside Blizzard's Edit Mode, positions per Edit Mode layout, and warnings when both place the same frame. | `editmode` | On |
| [Integrations](../showcase/features/interface.md#integrations) | Layouts place Details!, RestedXP guides, BigWigs bars and Questie's tracker, with an EldoUI look where the addon allows it. | `integrations` | On |
| [Buff and Consumable Reminders](../showcase/features/interface.md#buff-and-consumable-reminders) | A large icon when a class buff, gathering tracking or a chosen consumable is missing or running out. | `reminders` | On |
| [Counters](../showcase/features/interface.md#counters) | Watch items, currencies and gold as small movable counters, with goals and the session gain. | `counters` | On |
| [AFK Screen](../showcase/features/interface.md#afk-screen) | A calm screen with your character, zone, away time and whispers while you are marked Away. | `afk` | Off |
| [Macro Editor](../showcase/features/interface.md#macro-editor) | A wider macro editor with a live syntax check, a condition builder and an icon search. | `macros` | On |
| [Fanfare](../showcase/features/interface.md#fanfare) | Sounds, big text, screen flashes and icons for moments in the game: level up, epic loot, whispers, queue pops, boss kills and more. Fully customizable triggers. | `fanfare` | Off |

## Combat

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Unit Frames](../showcase/features/combat.md#unit-frames) | Player, target, focus, pet, target-of-target, boss, party pet and party target frames, plus Blizzard's own unit frames and cast bar. | `unitframes` | On |
| [Action Bars](../showcase/features/combat.md#action-bars) | Eight flat action bars, pet and stance bars, cooldown numbers, proc glow and fade rules. | `actionbars` | On |
| [Nameplates](../showcase/features/combat.md#nameplates) | Slim nameplates per unit type, with cast bar, your debuffs, quest and elite icons, style filters and a target highlight. | `nameplates` | On |
| [Buffs and Debuffs](../showcase/features/combat.md#buffs-and-debuffs) | Your buffs (right-click to cancel), debuffs, weapon enchants and boss mechanic auras, plus Blizzard's buff frames. | `auras` | On |
| [Class Resources](../showcase/features/combat.md#class-resources) | Health, power, combo points, druid mana and a GCD bar under your character, plus Blizzard's class resource frames. | `classpower` | On |
| [Aura Groups](../showcase/features/combat.md#aura-groups) | Your own rows of aura icons, each with its own mover: pick the spells, the unit and whether only yours count. The game shows each aura; EldoUI only places and dresses the icons. | `auragroups` | On |
| [Combat HUD](../showcase/features/combat.md#combat-hud) | Skins and places Blizzard's own combat displays: damage meter, swing timer, loss of control, mirror and quest timers, death recap. Plus EldoUI's threat meter, combat timer and cursor ring. | `combathud` | On |
| [Cooldown Manager](../showcase/features/combat.md#cooldown-manager) | Skins and places Blizzard's own Cooldown Manager (essential, utility, buff icons and buff bars). Blizzard keeps tracking every cooldown; EldoUI only changes the look and the position. Plus EldoUI's own rows (a fallback when Blizzard's has no spells, trinkets and mobility), which you can rearrange into your own groups and free icons with their own looks and labels. | `cooldownmanager` | On |
| [Quickdraw](../showcase/features/combat.md#quickdraw) | Hold a key for a ring, fan or grid of your own spells, items, macros, mounts and markers; let go on one to use it. | `quickdraw` | On |
| [Shaman Totems](../showcase/features/combat.md#shaman-totems) | Shamans: a totem bar with an element picker and Drop All, a shield and imbue cooldown bar, saved loadouts and party coverage. | `shamantotems` | Off |
| [Pet Care](../showcase/features/combat.md#pet-care) | Hunters: Feed Pet button next to the pet frame, unhappy pet and low food warnings. | `petcare` | On |
| [Danger Alerts](../showcase/features/combat.md#danger-alerts) | Sound alarms when you stand in something harmful (spell list), run out of breath or fatigue, or are attacked while AFK. | `alerts` | Off |
| [Enemy Spotter](../showcase/features/combat.md#enemy-spotter) | A small list of hostile players seen on nameplates, with class color, level and how long ago. | `enemyspotter` | Off |
| [Cast Tooltips and Mob Abilities](../showcase/features/combat.md#cast-tooltips-and-mob-abilities) | The spell tooltip on the target and focus cast bars, the abilities each mob cast in front of you, and reputation info on tokens. | `mobabilities` | On |
| [Spell Efficiency](../showcase/features/combat.md#spell-efficiency) | Damage or healing per second and per mana, and the mana cost as a share of your pool, on spell tooltips. | `spellefficiency` | On |

## Group

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Party and Raid](../showcase/features/group.md#party-and-raid) | Party, raid, main tank and pet frames with role, leader, status, aggro, buff, debuff, defensive and boss-mechanic indicators. | `groupframes` | On |
| [Click Casting](../showcase/features/group.md#click-casting) | Bind spells and macros to clicks on party, raid and unit frames, and see every binding in the frame's tooltip. | `clickcast` | On |
| [Raid Tools](../showcase/features/group.md#raid-tools) | A bar with ready check, role check, pull countdown, world markers, target icons and group tools for leaders and assists. | `raidtools` | On |
| [Dungeon Routes](../showcase/features/group.md#dungeon-routes) | Packs, patrols and bosses of the Classic dungeons on a map, with numbered pull routes you can edit, draw on, share and send to your group; the dungeon floor on the world map inside a dungeon, and an optional route card. | `dungeonroutes` | On |
| [Raid Loot](../showcase/features/group.md#raid-loot) | softres.it and That's My BiS imports on tooltips and loot rolls, and a GDKP ledger with sales, cuts and payouts. | `raidloot` | On |
| [Ready Check Report](../showcase/features/group.md#ready-check-report) | On a ready check, one panel lists each member's missing buffs, flask or elixir, food and shared durability, with one-click Post to group. | `readyreport` | On |
| [Party Quests](../showcase/features/group.md#party-quests) | In a group, compare your quests with your party (Shared, Only mine, Only theirs), with one-click Share and Ask and progress sync with members who run EldoUI (addon messages only, never chat). | `partyquests` | On |
| [Blessing Plan](../showcase/features/group.md#blessing-plan) | Plan which blessing each paladin keeps up on each class, then send the plan to the group or post it in chat with one click. | `blessingplan` | On |

## Chat and Social

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Chat](../showcase/features/chat-social.md#chat) | Chat on an EldoUI panel: clean tabs, clickable links, keyword alerts, saved history, search, a right panel and the error log. | `chat` | On |
| [Instant Messages](../showcase/features/chat-social.md#instant-messages) | Whispers (and, if you like, guild and group chat) in their own messenger windows, with contact info and a history browser. | `messages` | On |
| [Chat Bubbles](../showcase/features/chat-social.md#chat-bubbles) | Flat EldoUI speech bubbles with the EldoUI font, and control over which bubbles show, also in instances. | `chatbubbles` | On |

## Items and Economy

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Bags](../showcase/features/items-economy.md#bags) | All bags and the bank in EldoUI windows with categories and a bag bar, item counts across your characters, search with filters, offline viewing and a Blizzard skin mode. | `bags` | On |
| [Bag Actions](../showcase/features/items-economy.md#bag-actions) | Alt-click an item in your bags to disenchant it or pick its lock, with an exclude list and a quality cap. | `bagactions` | Off |
| [Loot Guide](../showcase/features/items-economy.md#loot-guide) | Loot journal, best-in-slot sets, wishlist and loot lines in item tooltips. | `lootguide` | On |
| [Attunements](../showcase/features/items-economy.md#loot-guide) | Attunements, keys and dungeon quest chains as a tab in the Loot Guide: a flowchart or step list per chain, progress for each of your characters, an optional guild view you ask for with a click, and step toasts. | `attunements` | On |
| [My Adventure](../showcase/features/items-economy.md#my-adventure) | Your character's journal as the first tab of the Journal window: a diary that writes itself, keepsakes, places, quests, companions, goals and notes, your story from 1 to 60, and where to go next. [Its own page](my-adventure.md). | `adventure` | On |
| [Upgrades](../showcase/features/items-economy.md#upgrades) | Upgrade arrows from a stat-weight scale: tooltips, bags, merchants, loot rolls and quest rewards. Pawn scale strings can be imported and exported. | `upgrades` | On |
| [Auction House](../showcase/features/items-economy.md#auction-house) | Shopping lists, quick selling with price checks, canceling, full scans, crafting costs and a price database for the auction house. | `auction` | On |
| [Merchant](../showcase/features/items-economy.md#merchant) | Repair, sell gray items, restock with exact amounts, fill ammo, and an item list for the merchant window. | `merchant` | On |
| [Mail](../showcase/features/items-economy.md#mail) | Open all, select and return letters, address book and a log of the mail you send. | `mail` | On |
| [Trade](../showcase/features/items-economy.md#trade) | Trade window look, mover, who you trade with, what each side's items are worth, and a gold trade log. | `trade` | On |
| [Mob and Loot Info](../showcase/features/items-economy.md#mob-and-loot-info) | Tracks what you loot from each mob and shows drop rates in item and mob tooltips. | `mobinfo` | On |
| [Appearances](../showcase/features/items-economy.md#appearances) | A small mark on item buttons in bags, vendors, loot, rolls and mail that says whether you have the item's look, and an "Appearance:" tooltip line. | `appearances` | On |
| [Profession Planner](../showcase/features/items-economy.md#profession-planner) | Pin recipes and see every reagent you need, what you have on all characters, a shopping list and a cheapest leveling plan. | `professionplanner` | On |
| [Zone Quests](../showcase/features/items-economy.md#zone-quests) | Every zone's done and remaining quests with their givers, optional quest giver pins on the world map and a quest count in the zone tooltip. | `zonequests` | On |
| [Quest Starter Drops](../showcase/features/items-economy.md#quest-starter-drops) | Creatures that can drop an item that starts a quest say so in their tooltip and with a small icon on their EldoUI nameplate. | `questdrops` | On |

## Quality of Life

| Module | What it does | `/eui` name | Default |
|---|---|---|---|
| [Quality of Life](../showcase/features/quality-of-life.md#quality-of-life) | Summon and resurrection prompts, social blocks, quest helpers and reward values, flight timer, durability figure, screen edge panels, sound and game settings. | `qol` | On |
| [Training](../showcase/features/quality-of-life.md#training) | What your class trainer can teach you now and later, with costs, totals, an ignore list, weapon skills and pet training. Its own window, a spellbook tab and an info bar block. | `training` | On |
| [Talent Planner](../showcase/features/quality-of-life.md#talent-planner) | Plan your talents, see the plan on Blizzard's talent page and learn the next point with one click. | `talents` | Off |
| [Legacy Planner](../showcase/features/quality-of-life.md#legacy-planner) | Plan Legacy points in a draft with a cost check, share profiles across characters, and browse challenges. Never spends a point. | `legacy` | Off |
| [Cast Bar Effects](../showcase/features/combat.md#cast-bar-effects) | Themed cast bars with sparks, trails, particles and finish effects, for EldoUI's and Blizzard's cast bars. | `castfx` | Off |
| [Instances](../showcase/features/group.md#instances) | Hourly instance count, a run log with stats, reset notices and a battleground log. | `instances` | Off |
| [Combat Text](../showcase/features/combat.md#combat-text) | Scrolling combat text in movable areas with notifications, nameplate numbers and a Blizzard hand-off. | `combattext` | On (new installs) |
| [Battleground Timers](../showcase/features/group.md#battleground-timers) | Queue, start, capture, winner and flag timers for battlegrounds. | `battlegrounds` | On |
| [Cooldown Pulse](../showcase/features/combat.md#cooldown-pulse) | A center pulse when your own spell or item is ready again. | `cdpulse` | Off |
| [Tracking Bars](../showcase/features/combat.md#tracking-bars) | One bar per spell for aura time, stacks, cooldown or charges, under the cooldown rows. | `trackingbars` | Off |
| [Consumable Bar](../showcase/features/combat.md#consumable-bar) | Your best food, drink, potions, bandage and healthstone on one small bar; one click uses one. | `consumablebar` | Off |
| [Encounter Timeline](../showcase/features/combat.md#encounter-timeline) | A small timeline that shows the timers your boss mod publishes as icons sliding towards now, with a big icon for the next one. | `encountertimeline` | On |
| [Alts](../showcase/features/items-economy.md#alts) | An Alts window with overview, search, professions, mail, quests, grids, level log and agenda for all your characters. | `alts` | Off |
| [Deadly Boss Mods](../showcase/features/interface.md#deadly-boss-mods) | Deadly Boss Mods with EldoUI's look, layout placement and quiet chat. | `dbm` | On |
| [Waypoints](../showcase/features/quality-of-life.md#waypoints) | `/way` coordinates, a direction arrow with distance and arrival time, and pins on the world map and minimap. | `waypoints` | On |
| [Bar Snapshots](../showcase/features/quality-of-life.md#bar-snapshots) | Save and restore action bars, macros and key bindings; automatic backups and a restore offer after a reset. | `snapshots` | On |
| [Camp Helper](../showcase/features/quality-of-life.md#camp-helper) | Campfire and feature tooltips, class-buff clashes, a camp panel with buff timers and a warning before Camp Benefits ends. | `camp` | On |
| [Quest Marks](../showcase/features/quality-of-life.md#quest-marks) | Tags and tints quests that are new in WoW: Forever in the quest window, quest log and quest giver lists. | `questmarks` | On |
| [Gathering](../showcase/features/quality-of-life.md#gathering) | Remembers your herb, ore and treasure finds and shows them on the world map and minimap. | `gathering` | On |
| [Map Notes](../showcase/features/quality-of-life.md#map-notes) | Rares and your own notes on the world map and minimap, and one button on the map that shows or hides every EldoUI pin (and HandyNotes). | `mapnotes` | On |
| [Rare Scanner](../showcase/features/quality-of-life.md#rare-scanner) | A click-to-target card and one sound when a rare shows up on the minimap, a nameplate, your target or in a yell; a tooltip line and a "Rares" data text. | `rarescanner` | On |
| [Zone Info](../showcase/features/quality-of-life.md#zone-info) | World map zone tooltip with level and gathering ranges, dungeons and territory, and an optional zone toast. | `zoneinfo` | On |
| [Farming](../showcase/features/quality-of-life.md#farming) | A farming session bar: time, looted gold, item value and XP per hour, sessions saved per zone. | `farming` | On |
| [Camera Situations](../showcase/features/quality-of-life.md#camera-situations) | The camera zooms to your distance at NPCs, in combat, mounted, indoors and in cities, and back afterwards. | `camera` | Off |
| [Player Notes](../showcase/features/chat-social.md#player-notes) | Your notes and Good/Avoid marks on players, on their tooltip, and a journal of who you grouped with. | `playernotes` | On |
| [Finder](../showcase/features/quality-of-life.md#finder) | One search box for game panels, EldoUI settings, mounts, toys, bag items, macros, places and commands. | `finder` | On |
| [Streamer Mode](../showcase/features/chat-social.md#streamer-mode) | Aliases in place of real character names on EldoUI's frames, tooltips and chat while you stream or record. | `streamermode` | On |
| [Chat Input](../showcase/features/chat-social.md#chat-input) | Long messages in parts you send one Enter at a time, a letter counter, undo and redo, and draft recovery. | `chatinput` | On |
| [Fishing](../showcase/features/quality-of-life.md#fishing) | Fishing mode: one key casts, then loots the bobber; a bar with Cast, Lure and Swap, and a catch log per spot. | `fishing` | Off |
| [Hardcore](../showcase/features/quality-of-life.md#hardcore) | For Hardcore characters: a death log, death alerts, a Tell the guild card, PvP-flag warnings and Self-Found reminders. | `hardcore` | On |
| [Split Timer](../showcase/features/quality-of-life.md#split-timer) | A leveling timer that races your own best, with a card at each level-up and a Splits tab in the Characters window. | `splittimer` | On |
| [Transport Maps](../showcase/features/quality-of-life.md#transport-maps) | Flight masters, boats, zeppelins, the tram and portals on the world map, with where each one goes. | `transport` | On |
| [Mage Travel](../showcase/features/quality-of-life.md#mage-travel) | For mages: one button that lists the teleports and portals you know with your rune counts; click a row to cast it. | `magetravel` | Off |
| [NPC Dialog](../showcase/features/quality-of-life.md#npc-dialog) | An optional dialog view for quest and gossip NPCs with big text, numbered choices, Space to go on and Esc to leave. | `dialogue` | Off |

## Earlier names

Some modules had another name in earlier versions. The old name still works in the config window's search and in `/eui`: Player Power (Class Resources), Micro Menu and Bags (Micro Menu and Bag Bar), Messages and Alerts and Messages (Alerts and Banners), Character (Character Panel), Sound and Fun (Fanfare), Characters (Alts), New in Forever (Quest Marks), and Tweaks, which is now part of Quality of Life.

## Plugins

Other addons can add modules of their own. They appear under **Plugins** in the sidebar and on the Plugins page (`/eui plugins`). See [Plugins](plugins.md).
