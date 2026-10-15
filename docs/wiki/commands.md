# Commands

Every command starts with `/eui` (or `/eldoui`). Names ignore case, and a unique start of a command is enough. `/eui help` opens the full list in game, built from the commands that are actually loaded, and `/eui help <command>` shows how to use one.

## General

| Command | What it does |
|---|---|
| `/eui` or `/eui options` | Open the config window |
| `/eui search <words>` | Open the config window with every setting that matches |
| `/eui help [command]` | The command list, or how to use one command |
| `/eui modules` | List the modules and whether they are on |
| `/eui <module> on`, `off`, `toggle` | Switch a module; `/eui <module>` alone opens its settings. `/eui enable <module>` and `/eui disable <module>` do the same |
| `/eui whatsnew` | What changed in this version |
| `/eui version` | The EldoUI version |
| `/eui install` | Run the setup wizard again |
| `/eui errors [clear]` | Show EldoUI's error log, or empty it |
| `/eui diag [copy]` | Version, modules, restrictions and secret values; `copy` gives text for a bug report |
| `/eui debug on`, `off` | Debug messages in chat |
| `/eui locale` | Language info |

## Layout and frames

| Command | What it does |
|---|---|
| `/eui move [on\|off]` | Unlock frames to drag them; again to lock |
| `/eui layout [name]` | Apply a layout preset; no name lists them |
| `/eui resetlayout` | Put every frame back to its layout position |
| `/eui scale auto` or `/eui scale <number>` | Automatic or your own UI scale |
| `/eui windows [lock\|unlock\|reset\|list]` | Move and scale Blizzard windows |
| `/eui blizz [element] [on\|off\|toggle]` | Which parts of Blizzard's UI EldoUI may change |
| `/eui editmode [conflicts\|layouts\|forget]` | EldoUI and Blizzard's Edit Mode |
| `/eui editlayout [copy]` | Copy Blizzard's active Edit Mode layout as text, or open the import window |
| `/eui infobar [show\|tab\|hide] [2]` | Show the Info Bar, fold it to a small tab or hide it (`2`: the second bar); alone it opens the Info Bar settings |
| `/eui kb` | Keybind mode: hover an EldoUI button and press a key |
| `/eui kb pro`, `classic`, `restore` | One-click keybind preset for every enabled bar, or put your old keys back |
| `/eui testframes [on\|off]` | Show every enabled unit frame with sample values |
| `/eui grouptest [party\|raid10\|raid20\|raid25\|raid40]` | Show or hide test party and raid frames |

## Profiles and sharing

| Command | What it does |
|---|---|
| `/eui profile` | List profiles; also `use <name>`, `copy <from>`, `reset`, `delete <name>` |
| `/eui renameprofile <new name>` | Rename the profile this character uses |
| `/eui copyparts <profile>` | Copy chosen modules from another profile |
| `/eui classprofile [<profile>\|none]` | The profile new characters of your class start with |
| `/eui profilerules on`, `off` | Switch profiles by talent group and content |
| `/eui export [all\|<module>]` | Export settings as a share string |
| `/eui exportlua [all\|<module>]` | Export settings as a readable Lua table |
| `/eui import` | Open the import window: EldoUI, EllesmereUI, ElvUI and Edit Mode strings, or a bundle of several strings at once |
| `/eui send <party\|raid\|guild\|player>` | Offer your settings to a group, guild or player |
| `/eui capture <addon>` | Save another addon's setup into EldoUI (Details, CooldownManager) |
| `/eui setup` | Set up every supported addon from EldoUI's profiles |
| `/eui plugins [list\|setup [name]]` | The Plugins page, a list in chat, or the plugins' setup pages again |

## Module commands

Commands that belong to one module.

| Command | Module | What it does |
|---|---|---|
| `/eui find <text>` | Bags | Search the items of all your characters |
| `/eui bank` | Bags | Show your saved bank anywhere |
| `/eui alts [search <text>\|agenda\|log\|size]` | Alts | The Alts window with all your characters: search their items, the agenda, the level log, or how much character data is saved |
| `/eui snapshot [list\|take [name]\|restore N\|rename N name\|export N\|delete N]` | Bar Snapshots | Save and restore your action bars, macros, key bindings and Edit Mode layout |
| `/eui macros` | Macro Editor | Open the EldoUI macro editor |
| `/eui go [text]` | Finder | Open the Finder search box: panels, settings, mounts, toys, items, macros and places |
| `/lg [text]`, `/eui guide`, `/eui lootguide` | Loot Guide | Open or close the Loot Guide |
| `/eui journey [section\|text]` | My Adventure | Open or close My Adventure, on a section or searched; also `data`, `report`, `check`, `export` and `import` ([all of them](my-adventure.md#commands)) |
| `/eui jot [text]` | My Adventure | Write a quick journal note here and now |
| `/eui adventure [on\|off\|toggle\|<section>]` | My Adventure | Switch My Adventure on or off, open its settings, or open a section |
| `/eui attune [name]` | Loot Guide | The Loot Guide on the Attunements tab, or one attunement by name |
| `/eui sim [bis\|char\|stop]` | Loot Guide | The Loot Guide simulator: open its window, or start or stop a run |
| `/eui tour lootguide`, `/eui tour journal` | Loot Guide | Start the Loot Guide or My Adventure tour again |
| `/eui newquest [questID]` | Quest Marks | Whether a quest is new in WoW: Forever; without an ID, the quest in the quest window |
| `/eui talents [next\|level\|export\|import\|send <party\|raid\|guild\|name>\|reset]` | Talent Planner | Open the Talent Planner, see your plan's next point, or share and reset a plan |
| `/eui legacy [challenges\|export\|import]` | Legacy Planner | Plan your Legacy points (it never spends them), browse challenges, or share a plan |
| `/eui plan [level\|pin <id> [n]\|unpin <id>\|clear]` | Profession Planner | Open the Profession Planner, or pin and unpin recipes |
| `/eui restock` | Merchant | Open the restock list |
| `/eui sentmail` | Mail | The log of mail you sent (at a mailbox) |
| `/eui trades` | Trade | The gold trade log |
| `/eui loothistory` | Loot | Open or close Blizzard's loot history |
| `/eui raidloot [ledger\|sr\|tmb\|clear\|post <item>]` | Raid Loot | Soft reserves, TMB lists and the GDKP ledger |
| `/eui farm [start\|pause\|stop\|reset\|history]` | Farming | The farming session bar and its history |
| `/eui gather [list\|clear [all]\|export [all]\|import\|send <who> [all]\|show]` | Gathering | The herb, ore, treasure and fishing nodes you have gathered |
| `/eui fish [mode\|log\|reset]` | Fishing | Fishing mode and the catch log |
| `/eui chatsearch <text>` | Chat | Search the selected chat window |
| `/eui chat mute <channel>` and more | Chat | Mutes, filters, colors and keyword alerts |
| `/eui eim [name]` | Instant Messages | The whisper history, or a conversation with a name |
| `/eui tt` | Chat | Whisper your target: opens the chat box as /w with its name |
| `/eui chatguild [mute <guild>\|unmute <guild>\|hidden]` | Chat | Muted guilds in chat; no word opens the list |
| `/eui note [Name [text]\|good Name\|avoid Name\|clear Name\|list]` | Player Notes | Your notes on other players |
| `/eui streamer [on\|off\|toggle]` | Streamer Mode | Show aliases in place of real names |
| `/eui party` | Party Quests | Show or hide the Party Quests panel |
| `/eui clickcast` | Click Casting | The click-casting bindings window |
| `/eui raidtools` | Raid Tools | Show the raid tools bar for a minute |
| `/eui pull [seconds\|cancel]` | Raid Tools | Start the group pull countdown (party, or lead or assist in a raid), or cancel it |
| `/eui timeline [test dungeon\|raid\|pull\|stop]` | Encounter Timeline | The timeline settings, or start and stop a test fight |
| `/eui dbm [setup\|undo\|apply\|test]` | Deadly Boss Mods | Set up Deadly Boss Mods with EldoUI's profile, switch back, apply it again, or show test timers |
| `/eui readycheck [post]` | Ready Check Report | Open the ready check report, or post its summary to the group |
| `/eui routes [dungeon\|import]` | Dungeon Routes | The dungeon map with packs and routes; a name opens that dungeon |
| `/eui instances [log\|add\|count\|stats\|pvp\|options]` | Instances | The run log and how many instances you entered this hour |
| `/eui deaths` | Hardcore | Open the Hardcore death log |
| `/eui quickdraw` | Quickdraw | The Quickdraw menu editor |
| `/eui hud` | Combat HUD | Combat HUD settings |
| `/eui threat [on\|off\|focus\|target]` | Combat HUD | EldoUI threat meter |
| `/eui meter [toggle\|reset]` | Combat HUD | Show or hide Blizzard's damage meter, or clear its fights |
| `/eui cursor [on\|off]`, `/eui crosshair [on\|off]` | Combat HUD | Cursor ring, crosshair |
| `/eui cdm [settings\|import\|capture]` | Cooldown Manager | EldoUI options, Blizzard's settings, import or capture this spec's set |
| `/eui ranks` | Action Bars | Move lower spell ranks on your bars to the highest rank you know |
| `/eui rankcheck` | Action Bars | List and light up the action buttons that hold a lower spell rank |
| `/eui castfx [test [theme] [seconds] [fail]\|dump]` | Cast Bar Effects | Open the page, play a test cast on every enabled cast bar, or list your spellbook with spell IDs |
| `/eui sct [test\|move]` | Combat Text | Combat Text settings, sample lines in every area, or move the scroll areas |
| `/eui notify test [lane\|errors\|warning\|bg\|pings]` | Alerts and Banners | Preview EldoUI's alerts and messages |
| `/eui cutscenes forget` | Alerts and Banners | Play every cutscene again once |
| `/eui map reset` | Maps | Put the world map, flight map and taxi window back where Blizzard places them |
| `/eui way [zone] x y [title]`, `/way` | Waypoints | Set a waypoint and follow the arrow; also `list`, `closest` and `reset [zone\|all]` |
| `/eui mapnote [on\|off\|add x y title\|hidden\|undo]` | Map Notes | Show or hide every EldoUI map pin, or add a map note |
| `/eui rares [test]` | Rare Scanner | Rare Scanner settings, or show a test card |
| `/eui camp [status\|panel\|announce\|ask\|share\|finds]` | Camp Helper | Campfire buffs, the camp panel, a one-line camp announcement and the camp finder |
| `/eui tracker on`, `off`, `toggle` | Quality of Life | Show or hide the quest tracker |
| `/eui volume` | Quality of Life | Show or hide the volume panel |
| `/eui wowhead` | Quality of Life | Wowhead address for what the tooltip shows, or your target |
| `/eui gamesettings` | Quality of Life | The game settings Quality of Life can change, and whether this client has them |
| `/eui cvars [name]` | Quality of Life | Browse every game setting (CVar), optionally at one setting |
| `/eui cam` | Camera Situations | The camera situation and distance right now |
| `/eui training [weapons\|config]`, `/wt` | Training | The Training window |
| `/eui afk test` | AFK Screen | Show the AFK screen for a moment |
| `/eui fx test <trigger>`, `list`, `mute` | Fanfare | Try a trigger, list them, or mute them |
| `/eui sound <id>`, `/eui media [type]` | Fanfare | Play a sound from the media library, or list the library |
