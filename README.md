# EldoUI

**An AI-made, deeply modular UI for WoW: Forever.**

EldoUI replaces and restyles the whole interface in one addon: unit frames, action bars, nameplates, bags, chat, maps, tooltips, and much more. Every part is a module you can turn on or off on its own. Pick one of 17 layout presets, move anything you like, and keep one consistent look across every window.

EldoUI is built with AI assistance, and it is designed and tested for WoW: Forever.

## Highlights

- **More than 90 modules.** Turn every module on or off with one click or one command. Anything you switch off leaves Blizzard's own version in place.
- **20 layout presets.** Each one places every frame on a 1440p canvas, in one click. The layouts look the same on 1080p, 1440p, and 4K, and an ultrawide safe area keeps the UI centered.
- **Move and style everything.** `/eui move` unlocks every frame with grid snap and pixel nudging. Style presets and art styles change the look, never the position.
- **One config window.** Search finds any setting by name, description, or choice. Changed rows are marked, and a Recent changes list lets you undo.
- **Guided setup.** A step-by-step installer picks your scale, layout, role, modules, and chat setup on the first login.
- **Profiles and sharing.** Account and character profiles, profiles per talent group, and share strings for a whole setup or a single module. Imports from EllesmereUI, ElvUI, and Edit Mode strings.
- **Plays well with others.** One-click setups for Details!, BigWigs, Deadly Boss Mods, and the Cooldown Manager. A module steps aside when another addon already does the same job.
- **Fair play.** EldoUI only changes how the interface looks and where things sit, and shows only what the game gives addons. It never plays for you, and nothing acts without your click unless you turn it on.

## What is inside

| Area | Modules |
|---|---|
| Frames | Unit Frames, Party and Raid with click casting, Class Resources, Buffs and Debuffs, Aura Groups, Nameplates, Action Bars |
| Combat | Combat HUD, Cooldown Manager, Combat Text, Encounter Timeline, Cast Bar Effects, Tracking Bars, Cooldown Pulse, Danger Alerts |
| Interface | Info Bar, Minimap, Maps, Quest Tracker, Tooltip, XP and Reputation Bars, Alerts and Banners, Edit Mode support, skins for Blizzard's windows |
| Chat and social | Chat with history and search, Instant Messages, Chat Bubbles, Chat Input, Player Notes, Streamer Mode |
| Items and economy | Bags and bank across your characters, Upgrades, Auction House, Merchant, Mail, Trade, Appearances, Profession Planner |
| Guides | Loot Guide, My Adventure journal, Zone Quests, Training, Talent Planner, Dungeon Routes |
| Quality of life | Waypoints, Map Notes, Rare Scanner, Gathering, Fishing, Finder, Macro Editor, and more |

The [feature showcase](docs/showcase/overview.md) describes every module, and the [module list](docs/wiki/modules.md) shows which ones start on.

## Install

1. Download `EldoUI-<version>.zip` from the [releases page](https://github.com/Eldodeldo/EldoUI/releases).
2. Close the game and unzip the file into `World of Warcraft\_classic_beta_\Interface\AddOns`.
3. Check that these folders sit directly in `AddOns`: `EldoUI`, `EldoUI_LootData`, `EldoUI_LootSim`, and `EldoUI_Emoji`.
4. Start the game, make sure **EldoUI** is ticked in the AddOns list, and log in.

The three companion folders load only when you need them: the Loot Guide data, the gear simulator, and the chat emoji.

### Updating

Close the game, delete the old EldoUI folders, and unzip the new version. Your settings live in the game's `WTF` folder, so an update never loses them. See [Updating](docs/wiki/updating.md) for details.

## First start

The installer opens on your first login. It walks you through the UI scale, a layout, style presets, your role, the addons you already use, the modules you want, Blizzard's own UI, chat, and other addons. Nothing changes until you click Apply or Finish, and `/eui install` runs it again at any time.

New to EldoUI? Start with [Getting started](docs/wiki/getting-started.md).

## Commands

| Command | What it does |
|---|---|
| `/eui` | Open the config window |
| `/eui help` | Show every command in game |
| `/eui move` | Unlock frames to drag them; run it again to lock |
| `/eui layout <name>` | Apply a layout preset; `/eui layout` alone lists them |
| `/eui <module> on` or `off` | Turn a module on or off, for example `/eui nameplates off` |
| `/eui kb` | Keybind mode: hover a button and press a key |
| `/eui export` and `/eui import` | Share your setup as a string |
| `/eui errors` | Show EldoUI's error log |

The [command reference](docs/wiki/commands.md) lists all of them.

## Compatibility

- **Game:** WoW: Forever (Interface 16001). EldoUI does not run on Classic Era or Retail.
- **Languages:** English. The Loot Guide is also translated into German, French, Spanish, Brazilian Portuguese, Russian, Korean, and Chinese.
- **Other addons:** EldoUI works next to Details!, BigWigs, Deadly Boss Mods, Questie, RestedXP, HandyNotes, and Masque. It notices the addons you already use for bags, bars, frames, chat, and more, and steps back where they do the same job: a whole module (Bags while Bagnon is loaded) or only the parts both do (selling gray items with Leatrix Plus). You pick who handles each job on the Other addons page, with `/eui addons`, or in the setup. See [Using EldoUI with other addons](docs/wiki/other-addons.md).

## Documentation

- [Getting started](docs/wiki/getting-started.md)
- [Updating](docs/wiki/updating.md)
- [Modules](docs/wiki/modules.md)
- [Layouts and presets](docs/wiki/layouts.md)
- [My Adventure](docs/wiki/my-adventure.md)
- [Commands](docs/wiki/commands.md)
- [FAQ](docs/wiki/faq.md)
- [Plugins](docs/wiki/plugins.md) and the [plugin guide](docs/PLUGINS.md) for addon authors
- [Changelog](CHANGELOG.md)

## Reporting bugs

1. Type `/eui errors` to open EldoUI's error log.
2. Press Report on the error. It shows a ready-to-paste bug report with the version and setup details, and with your character's name, realm, guild and chat text left out.
3. Open the [bug form](https://github.com/Eldodeldo/EldoUI/issues/new?template=bug_report.yml) and paste it in, with a few words on what you were doing.

EldoUI never sends anything by itself: a report leaves the game only when you paste it.

`/eui diag copy` gives you the version and setup details on their own. The [FAQ](docs/wiki/faq.md#how-do-i-report-a-problem) has more tips.

## For addon authors

Plugins add their own modules to EldoUI through the global `EldoUI` and get a settings page, an installer step, and the same look as the rest of the UI. See the [plugin guide](docs/PLUGINS.md).

## Credits

EldoUI stands on the work of the WoW addon community. It embeds LibStub, CallbackHandler-1.0, and LibActionButton-1.0, ships open fonts and sounds, uses loot data from CMaNGOS classic-db, and adapts open-source code from What's Training?, Molinari, and Forever Journal. Many features were inspired by addons such as ElvUI, EllesmereUI, Plater, Details!, and Leatrix Plus. Thank you to all of their authors.

The full list, with every license, is in [Credits and third-party notices](THIRD_PARTY_NOTICES.md) and the [media credits](LICENSES/Media.md).

## License

Copyright 2026 Eldodeldo. EldoUI is licensed under the [Apache License, Version 2.0](LICENSE) (see also [NOTICE](NOTICE)).

Bundled libraries, adapted code, data, fonts, and sounds keep their own licenses. The `EldoUI_LootData` folder is licensed under GPL-3.0-or-later because its data comes from CMaNGOS classic-db.
