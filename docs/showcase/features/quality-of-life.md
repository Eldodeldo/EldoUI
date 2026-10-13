# Quality of Life

Small helpers that save clicks and windows that tell you more.

[Back to the overview](../overview.md)

## Quality of Life

One page with five tabs. **Interface**: Wowhead links for what the tooltip shows (`/eui wowhead`), XP bar text, +/- Combat text, Blizzard's durability figure on a mover and thin screen edge panels. **Social**: clear prompts for summons and resurrections (you still click Accept), social blocks and chat filters. **Quests**: a quest tracker toggle (`/eui tracker`), zone tracking in the quest log, quest helpers that accept and turn in for you (off until you turn them on, never pick a reward) and sell values on quest rewards. **Travel**: a flight timer that shows the route, stops and arrival time. **Sound and misc**: a volume panel (`/eui volume`), sound and graphics comforts, camera and screenshot settings, shortcuts to game settings such as self-cast and the spell queue window, and a browser of every game setting (`/eui cvars`). `/eui gamesettings` lists the game settings it can change and whether this client has them. This page was two modules before, Quality of Life and Tweaks; `/eui tweaks` still opens it.

## Training

What your class trainer can teach you now and later, with costs, totals, an ignore list, weapon skills and pet training. It has its own window (`/eui training` or `/wt`), a spellbook tab and an info bar block. Data adapted from What's Training?.

> Screenshot coming soon: the Training window with spells available now and later.

## Talent Planner

Plan your own class's talents in a window with three tabs: the trees, a level-by-level guide and your saved plans (one per talent group). Your plan shows on Blizzard's talent page. When you have a free point, a reminder offers "Learn next", and EldoUI learns only when you click. Plans share as `!EUT1!` strings or chat links. `/eui talents` or a key binding opens the planner.

## Legacy Planner

Plan your Legacy points without touching them (`/eui legacy`). Copy your current build into a draft, add or remove ranks, and see every change in color next to what you have, with a cost line that warns when the draft needs more points than you own or goes over the season cap. Save drafts as named profiles that all your characters can load, and share them as a string. The Challenges page lists every challenge with progress bars, status chips, a category menu and a search. With the Blizzard UI switch for the Legacy window on Improve, the planner docks beside Blizzard's Legacy window. A Legacy column shows each character's points in Characters. EldoUI never spends, refunds or commits a point.

## Waypoints

Type `/way 45 63 Goldshire` or `/way Elwynn Forest 41 65`, or Ctrl+right-click on the world map, to set a waypoint. An arrow in EldoUI's look points the way and shows the distance and arrival time, and pins show on the world map and minimap. Waypoints are kept per character, and the game's own map pin follows the arrow. In dungeons, where the game hides your position, the arrow says so. After you release your spirit, the arrow points to your corpse. `/way paste` takes many /way lines at once, for example from a guide.

## Bar Snapshots

Saves what is on every action slot, your macros and your key bindings, and puts them back with one click (`/eui snapshot`). Snapshots are taken at login and logout when something changed. If the game comes up with empty bars, EldoUI offers to restore them. Snapshots can be exported as a string for another character.

## Camp Helper

Makes WoW: Forever camps easy to read (`/eui camp`). Hovering a campfire shows its tier, its slots and the features you have seen around it; hovering a feature shows what its buff gives, whether you have it and for how long, and which class buff blocks it (camp buffs never stack with their class version, such as the Incense Candle and Arcane Intellect). A small camp panel (move it in move mode) lists your camp buffs with timers, the shared one-hour feature cooldown and the tent lockout, and shows only near a fire or while a camp buff is on you. A note comes before Camp Benefits ends. The panel's Announce button posts one line about the camp to /say or /party when you click it. The game has no list of a camp's objects, so the counter shows the features you have hovered.

## New in Forever

Marks quests that are new in WoW: Forever. A new quest gets a small "New in Forever" tag and a tinted title in the quest window, and is tinted in the quest log and in a quest giver's list. A quest counts as new when its ID is one the original game never used (and, with the Loot Data folder loaded, when that list doesn't have it). Pick the color and tag text, or a style: Teal, Gold "New", Tag only or Subtle. `/eui newquest 12345` tells you about any quest ID.

## Gathering

Remembers every herb, ore vein and chest you gather and shows the nodes as pins on the world map and minimap (`/eui gather`). Finds of the same node close together count as one node, with how often you gathered it and when you last did. Pins can be profession icons or small colored dots; filter by herbs, ore and treasure, keep far nodes on the minimap's edge, and right-click a pin to set a waypoint there or forget the node. Only your own finds are shown.

## Map Notes

A small button at the top right of the world map shows or hides every EldoUI pin at once: your own notes, rares, waypoints, gathering nodes and instance entrances, and HandyNotes with its plugins when it is installed (`/eui mapnote`, or a key binding). Click it for one tick per group, with how many pins each has on the map you're looking at; Shift-click flips everything. The same ticks sit in the map's own filter menu. Rares from the Loot Guide's data show their level and drops, with Collected marks for mounts, pets, toys and appearances, and hide themselves once you have everything they drop. Alt+right-click on the map adds your own note with a title, a note, an icon and an option to show it on the continent map. Right-click any pin to set a waypoint, put a map link in the chat box, or hide that point. Seven style presets (Standard, Game icons, Quiet dots, Loot icons, Large, Treasure hunter, World map only).

## Rare Scanner

Tells you when a rare creature shows up, from what the game itself shows: a skull on the minimap, a nameplate, your target, the creature under your mouse, a party member's target or a yell from a rare you know of. You get one card left of the top center and one sound (a second sound for a rare that drops a mount, pet or toy you don't own yet). Click the card to target the rare; Shift-click puts its name and place in the chat box for you to send, Alt-click shows it on the map, right-click or x closes it. In combat a short note says the card opens after combat. A tooltip line marks rares and when you saw them this session, and the "Rares" data text lists this session's sightings. Optional: a chat line, raid marking on your own click, and a targeting key you press yourself. Nothing is kept after you log out except your settings and the rares you chose to ignore. Six style presets (Standard, Compact, Minimal, Showcase, Rare hunter, Quiet). `/eui rares`, `/eui rares test`.

## Zone Info

Hover a zone on the world map to see its level range, the Herbalism, Mining, Skinning and Fishing ranges colored by your own skill, its dungeons (with the ones new in Forever marked) and whose territory it is. Hold Shift to list the node types you have found there with Gathering. An optional zone toast shows the same facts when you enter a new zone, in six styles.

## Farming

A farming session bar (`/eui farm`, and a Farming info bar text). It starts on your first loot, or with a click, and counts the time, the gold you loot, the items you loot and their worth (vendor price, your saved auction prices, or the higher of both) and the XP you gain, each also per hour. Money from merchants, mail, trades, the auction house, the bank and quest rewards is not counted. The timer pauses while you are away. Stopping saves the session under the zone, and the tooltip shows your best gold per hour there and the most valuable items of the session. An optional gold goal gives a note and a sound.

## Camera Situations

The camera zooms to your own distance for each situation: talking to an NPC, in combat, mounted or on a flight, indoors, in a city or inn, and out in the world. The first situation that applies wins, in that order; when none applies, the camera goes back to the distance you had. Only the camera distance changes. Five style presets (Standard, Cinematic, Overview, Indoors only, Talk). Off by default; turn it on under Quality of Life. `/eui cam` shows the situation and distance right now.

## Finder

One search box (`/eui go`, or a key you choose) for game panels, EldoUI settings, mounts, toys, bag items, macros, places and EldoUI commands, with pins and recent results. Using a mount, toy, item or macro is always your own click or Enter, and never in combat.

## Fishing

Turn on fishing mode and the key you choose casts Fishing, then loots the bobber while it is out; each press is one action, and nothing casts by itself. A small bar has Cast, Lure (your best lure) and Swap (pole or weapons back). An optional louder splash makes the bite easy to hear, and the game's sound settings come back afterwards. The catch log keeps what you caught per zone and spot, catches per hour and skill-ups. `/eui fish`.

## Hardcore

On Hardcore characters only: a log of the deaths the game announces, death alert cards, and after your own death a card with a one-click "Tell the guild". It warns before you attack or help a PvP-flagged target and when you get flagged, and Self-Found characters get reminders at the mailbox, auction house and trade window. `/eui deaths`.

## Split Timer

A small leveling timer shows your time on this level and the difference to your best: your best per level, your personal best or a character you pick. Each level-up shows that level's time against the best, and the Characters window gets a Splits tab to compare characters. It uses only your level log and /played.

## Transport Maps

The world map shows flight masters, boats, zeppelins, the tram and fixed portals for your side, each kind with its own shape and color. Flight masters and their "not found yet" state come from the game; where each one flies is learned when you open its flight map, and learned flight times show in the tooltip. Right-click a stop to set a waypoint. The Routes tab lists the stops of a zone, where each goes and what arrives there. Taking a flight is always your own click at the flight master.

## NPC Dialog

Quest and gossip NPCs talk in a large, readable view: keys 1 to 9 pick a choice, Space shows the whole text and then goes on, R shows rewards and Esc leaves. It never accepts, completes or picks anything for you; a page with several rewards waits for your pick. In combat and for special frames the game's own window is used.
