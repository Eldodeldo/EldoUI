# Interface

The frames around the edges of your screen, Blizzard's windows in the EldoUI look, and the messages the game shows you. Every module here has its own page in `/eui` and can be switched off with `/eui <module> off`.

[Back to the overview](../overview.md)

## Info Bar

Full-width bars at the top or bottom of the screen and your own datatext panels anywhere you like. Datatexts show the clock, gold, durability, latency and FPS, your stats, currencies, your hearthstone and more; addons that publish LibDataBroker feeds show up as datatexts too. A second bar and free panels let you split them up, and a battleground swap shows battleground info while you are in one.

## Minimap

A square or round minimap with zone text, coordinates and a clock, rebuilt behind Blizzard's minimap. You decide where the minimap buttons sit, and an addon button bin gathers other addons' buttons in one place. The minimap buttons and the queue button have their own Blizzard switches. With the Vanilla Original skin, a round minimap wears the game's own classic border, scaled with the map.

## Tooltip

Clean tooltips in the game's own style with quality and class-colored borders, a tidy info area and a movable anchor (or a Smart position that keeps out of your way). Extra lines show what the game gives addons: gathering skill, mount source and who is targeting a unit. Other modules add their own sections, such as the Loot Guide's drop lines.

## Maps

The world map, quest log, flight map, battlefield map and UI widgets with an EldoUI skin, your own position and scale, coordinates and fading while you move. The world map can show the level range of the zone under the cursor. `/eui map reset` puts them back where Blizzard places them.

## Quest Tracker

Blizzard's quest and objective tracker in the EldoUI look, on its own mover, with your height and font. It can fade or fold up in combat, shows a button and a key for the tracked quest's item, and works with Questie's tracker.

## XP and Reputation Bars

Experience with rested XP, reputation, honor and pet experience bars in one movable stack. Ticks, upright bars, hiding in combat, click panels and automatic tracking of the reputation you just gained are all options.

## Micro Menu and Bag Bar

Move, resize and restyle Blizzard's micro menu and bag bar, or fold them into the Info Bar and the bag window. Gaps close on their own when buttons show or hide.

## Alerts and Banners

Toasts, banners and the talking head, raid warnings, the red error text, zone text, ready checks, queue pop-ups and cutscenes, each in the EldoUI look and placed by your layout. EldoUI's alert lane shows its own messages in one place, and pings get a short feed. `/eui notify test` previews them.

## Loot

The loot window, group roll bars, loot history and loot toasts in the EldoUI look. Rolls stay fully manual: EldoUI never rolls for you. A loot feed mode turns the toasts into a running list.

## Character Panel

The character window, its slots and side panels in the EldoUI look, with item level, a classic or modern stats layout and stat sections you can fold. Gear set buttons equip a set on a click.

## Friends and Social

The friends, guild, calendar, group finder and PvP windows in the EldoUI look, with class colors, a friends search and movable windows.

## NPC Windows

Quest, gossip and other NPC dialogs, the pet stable and the barber shop in the EldoUI look.

## Window Skins

The spellbook, talents, professions, trainer, collections, socketing, dressing room and inspect windows in the EldoUI look, plus the option windows of other addons built with Ace3.

## System Windows

The game menu, Settings, the AddOn list, key bindings, macros and pop-ups in the EldoUI look, with a few safe extras.

## Edit Mode

EldoUI's frames inside Blizzard's Edit Mode, positions saved per Edit Mode layout, and a warning when EldoUI and Edit Mode both try to place the same frame. `/eui editmode conflicts` lists them.

## Integrations

Layouts also place Details!, RestedXP guides, BigWigs bars and Questie's tracker, with an EldoUI look where the addon allows it.

## Buff and Consumable Reminders

A large icon when a class buff, gathering tracking or a consumable you chose is missing or running out. Rules can follow the content you are in, and a click casts the missing buff where the game allows it. It reads auras only out of combat.

## Counters

Watch items, currencies and gold as small movable counters, with a goal and what you gained this session.

## AFK Screen

A calm screen with your character, zone, time away and the whispers you got while you are marked Away. Off by default; `/eui afk test` shows it for a moment.

## Fanfare

Sounds, big text, screen flashes and icons for moments in the game: level up, epic loot, whispers, queue pops, ready checks, boss kills, rares and more. Every trigger can be changed or switched off, and the media library lets you pick any sound, including SharedMedia ones. Off by default; `/eui fx test <trigger>` plays one.

## Deadly Boss Mods

Deadly Boss Mods with an EldoUI touch: its own DBM profile per layout, timers and warnings placed by the layout, the EldoUI look and quiet chat. Your DBM profile, sounds and boss settings stay yours. Only active while Deadly Boss Mods is installed.

## Macro Editor

A wider editor next to Blizzard's macro window (`/eui macros`, or "Edit in EldoUI"). It checks the macro as you type, has a condition builder that inserts at the cursor, finds icons by spell or item name and duplicates macros. Saving happens out of combat, and the editor never runs a macro.
