# Group

Frames and tools for playing with others.

[Back to the overview](../overview.md)

## Party and Raid

Party, raid, main tank and pet frames with role, leader, status, aggro, buff, debuff, defensive and boss-mechanic indicators. Each section (party, raid sizes, main tanks, pets) has its own layout, text tags, fades, aura filters, glows and heal prediction. `/eui grouptest party` (or `raid10`, `raid20`, `raid25`, `raid40`) shows test frames so you can place and style them.

> Screenshot coming soon: a 5-player party and a 20-player raid with test frames in the Eldo-Modern layout.

## Click Casting

Bind spells and macros to clicks on party, raid and unit frames, and see every binding in the frame's tooltip. `/eui clickcast` opens the bindings window.

## Raid Tools

A bar for leaders and assists with ready check, role check, a pull countdown, world markers, target icons and group tools. `/eui raidtools` shows it for a minute.

## Instances

Counts your dungeon and raid entries against the hourly instance limit (5 per hour, across every character on the same ruleset, shown as an estimate), with an info bar block that says when the next slot frees up. A run log lists every run with time, XP, kills, gold and reputation, and a battleground tab lists your battlegrounds with result and honor. Walking back into the same instance merges the runs. Reset notices tell you and your group what was reset, and Raid Tools can get a Reset instances button. `/eui instances` opens the log.

## Battleground Timers

Timer bars for battlegrounds: queue time against the game's estimate, time to enter, battle start, base captures from the map, the expected winner and time left from the score widgets, and when a flag is back. Skins, moves or hides Blizzard's start countdown. Shift-click puts a bar's text in the chat box (it never sends on its own). Steps back for DBM-PvP and Capping. `/eui probe bg` prints the battleground's widgets and map points, and keeps the last 20 of these reports in the SavedVariables file (`/eui probe bg clear` removes them).

## Dungeon Routes

A Dungeons window (`/eui routes`) shows the packs, patrols and bosses of all 26 Classic dungeons and wings on the dungeon map or a schematic view. Pack markers show how many mobs a pack has, with a gold ring for elites; bosses are numbered in order, and patrols show their path. Each dungeon comes with a full-clear route of numbered, colored pulls. Copy it as your own route or start an empty one, then edit it on the map: click packs to add or take out pulls, drag pulls to reorder them, label and color them, and write notes, draw arrows and free-hand lines (with undo). Share a route as a string, or send it to your group with one click; with "Get routes your group sends" turned on (off by default), routes others send wait in a From your group list until you keep one. Nothing is ever sent back.

Inside a dungeon, the world map (M or any map button) shows the dungeon's floor with its packs and your route instead of the game's empty instance map, with floor buttons, a Game map button, and your dot only when the game gives your position. An optional route card (off by default, movable in `/eui move`) lists the next pulls; tick them off with Done and the next pull is lit on the map. The same packs and route show on the Loot Guide's dungeon map. The data comes from the EldoUI_LootData folder; dungeons it lacks can get hand-placed packs. It is planning only: nothing is pulled, targeted or marked for you.

## Raid Loot

Paste a softres.it or That's My BiS export and every item tooltip and loot roll shows who reserved it ("SR:") or has it on their list ("TMB:"); the Loot Guide marks the items you reserved. A GDKP ledger keeps each sale, the pot, cuts and every player's payout, with a text export. Posting a line to the group is one click and off by default, and EldoUI never rolls, trades or bids for you. `/eui raidloot`.

## Ready Check Report

When a ready check starts, one panel shows what each member is missing: class buffs, flask or elixir and Well Fed, read out of combat only. Durability and the EldoUI version show for members who choose to share them (off by default). "Post to group" sends one summary line per click. `/eui readycheck`.

## Party Quests

An optional panel in a group compares your quest log with your party in three cards: Shared, Only mine and Only theirs. Share uses the game's own quest share; Ask sends one whisper per click and is never answered automatically. Party Quests is on by default, and so is "Sync with group": it shares your quest progress with group members who also use EldoUI, as addon messages only, never chat, for progress popups and a summary when the group ends. It stays silent in battlegrounds and arenas, and in raids while Hide in raids is on (the default). `/eui party`.
