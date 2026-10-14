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
| `/eui import` | Open the import window: EldoUI, EllesmereUI, ElvUI and Edit Mode strings |
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
| `/lg [text]`, `/eui guide`, `/eui lootguide` | Loot Guide | Open or close the Loot Guide |
| `/eui journey [section\|text]` | My Adventure | Open or close My Adventure, on a section or searched; also `data`, `report`, `check`, `export` and `import` ([all of them](my-adventure.md#commands)) |
| `/eui jot [text]` | My Adventure | Write a quick journal note here and now |
| `/eui restock` | Merchant | Open the restock list |
| `/eui sentmail` | Mail | The log of mail you sent (at a mailbox) |
| `/eui trades` | Trade | The gold trade log |
| `/eui loothistory` | Loot | Open or close Blizzard's loot history |
| `/eui chatsearch <text>` | Chat | Search the selected chat window |
| `/eui chat mute <channel>` and more | Chat | Mutes, filters, colors and keyword alerts |
| `/eui eim [name]` | Instant Messages | The whisper history, or a conversation with a name |
| `/eui clickcast` | Click Casting | The click-casting bindings window |
| `/eui raidtools` | Raid Tools | Show the raid tools bar for a minute |
| `/eui pull [seconds\|cancel]` | Raid Tools | Start the group pull countdown (party, or lead or assist in a raid), or cancel it |
| `/eui timeline [test dungeon\|raid\|pull\|stop]` | Encounter Timeline | The timeline settings, or start and stop a test fight |
| `/eui quickdraw` | Quickdraw | The Quickdraw menu editor |
| `/eui hud` | Combat HUD | Combat HUD settings |
| `/eui threat [on\|off\|focus\|target]` | Combat HUD | EldoUI threat meter |
| `/eui meter [toggle\|reset]` | Combat HUD | Show or hide Blizzard's damage meter, or clear its fights |
| `/eui cursor [on\|off]`, `/eui crosshair [on\|off]` | Combat HUD | Cursor ring, crosshair |
| `/eui cdm [settings\|import\|capture]` | Cooldown Manager | EldoUI options, Blizzard's settings, import or capture this spec's set |
| `/eui ranks` | Action Bars | Move lower spell ranks on your bars to the highest rank you know |
| `/eui notify test [lane\|errors\|warning\|bg\|pings]` | Alerts and Banners | Preview EldoUI's alerts and messages |
| `/eui cutscenes forget` | Alerts and Banners | Play every cutscene again once |
| `/eui map reset` | Maps | Put the world map, flight map and taxi window back where Blizzard places them |
| `/eui tracker on`, `off`, `toggle` | Quality of Life | Show or hide the quest tracker |
| `/eui volume` | Quality of Life | Show or hide the volume panel |
| `/eui wowhead` | Quality of Life | Wowhead address for what the tooltip shows, or your target |
| `/eui gamesettings` | Quality of Life | The game settings Quality of Life can change, and whether this client has them |
| `/eui training [weapons\|config]`, `/wt` | Training | The Training window |
| `/eui afk test` | AFK Screen | Show the AFK screen for a moment |
| `/eui fx test <trigger>`, `list`, `mute` | Fanfare | Try a trigger, list them, or mute them |
| `/eui sound <id>`, `/eui media [type]` | Fanfare | Play a sound from the media library, or list the library |
