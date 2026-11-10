# EldoUI

**An AI-made, deeply modular UI for WoW: Forever.**

EldoUI replaces and restyles the whole interface in one addon: unit frames, action bars, nameplates, bags, chat, maps, tooltips, and much more. Every part is a module you can turn on or off on its own. Pick one of eleven layouts and the role you play, move anything you like, and keep one consistent look across every window.

EldoUI is built with AI assistance, and it is designed and tested for WoW: Forever.

## EldoUI 0.7.1000

This README and the [player guide](docs/wiki/getting-started.md) describe the 0.7.1000 setup. Get published downloads from the [releases page](https://github.com/Eldodeldo/EldoUI/releases). [Current release](docs/wiki/current-release.md) provides the release-note reference.

- **98 modules.** Choose the parts you want in the config window or with a command. Supported replacements restore Blizzard's interface when turned off; optional helpers simply stop.
- **Eleven current layouts, four roles.** Start with EldoUI Center or choose another layout, with automatic scaling from a 1440-unit reference canvas and screen-area controls for ultrawide displays. Melee, Ranged, Healer and Tank add role settings; Healer offers group-frame positions and Tank adds threat colors. Check the layout and style previews for your screen and settings.
- **Guided setup.** A step-by-step setup picks your scale, layout, look, role, modules, chat and keys on the first login, or sets up everything at once from a preset pack. Short tour helps explain new parts the first time you meet them.
- **Your keys, your way.** A key set that belongs to your profile and knows US, UK, Nordic, German and French keyboards. The Keys and spells step shows your keys, class spells and macros first and changes nothing on your bars until you press Apply.
- **Your layout and look.** `/eui move` opens the available movers, with grid snap and pixel nudging. Fourteen skins set the art, module styles set details such as size and text, and preset packs combine a layout, look and settings. Your dragged positions stay unless you choose to reset them.
- **Undo when you change your mind.** Every layout or pack change can be undone from the alert after the change or with `/eui layout undo`, and a Recent changes list in the config window undoes single settings.
- **One config window.** Search finds any setting by name, description, or choice, and changed rows are marked.
- **[Eldostar](docs/wiki/eldostar.md) and [My Adventure](docs/wiki/my-adventure.md).** EldoUI's own guide window follows community guides, with step controls and a waypoint to the next goal. The Journal brings together your character's story, dungeon runs, quests, keepsakes and notes.
- **Profiles and sharing.** Account and character profiles, profiles per talent group, and share strings for a whole setup or a single module. Imports EllesmereUI, ElvUI, and Edit Mode strings.
- **Saved data and backups.** Settings and journals live separately from the addon files. `/eui data` lists copies kept before saved-data updates and lets you restore them; the journal also has backup and export controls.
- **English and Danish.** EldoUI's own texts can be shown in Danish, under General > EldoUI language.
- **Other addon choices.** Setup offers profiles for supported addons such as Details! and BigWigs. The Other addons page lets you choose who handles recognized overlapping jobs.
- **Fair play.** EldoUI only changes how the interface looks and where things sit, and shows only what the game gives addons. It never plays for you, and nothing acts without your click unless you turn it on.

What changed in each release is in the [changelog](CHANGELOG.md). Version 0.7.1000 starts with a fresh EldoUI profile and eleven built-in presets. Profile and preset updates are supported from this version onward.

## What is inside

| Area | Modules |
|---|---|
| Frames | Unit Frames, Party and Raid with Click Casting, Class Resources, Buffs and Debuffs, Aura Groups, Nameplates, Action Bars |
| Combat | Combat HUD, Cooldown Manager, Combat Text, Encounter Timeline, Cast Bar Effects, Tracking Bars, Cooldown Pulse, Consumable Bar, Danger Alerts |
| Interface | Info Bar, Minimap, Maps, Quest Tracker, Tooltip, XP and Reputation Bars, Micro Menu and Bag Bar, Alerts and Banners, Edit Mode, skins for Blizzard's windows |
| Chat and social | Chat with history and search, Instant Messages, Chat Bubbles, Chat Input, Player Notes, Streamer Mode |
| Items and economy | Bags and bank across your characters, Upgrades, Auction House, Merchant, Mail, Trade, Appearances, Profession Planner, Alts |
| Guides | Eldostar, Loot Guide with Attunements, the My Adventure journal, Zone Quests, Training, Talent Planner, Legacy Planner, Dungeon Routes |
| Group | Raid Tools, Ready Check Report, Party Quests, Raid Loot, Blessing Plan, Battleground Timers, Instances |
| Quality of life | Waypoints, Map Notes, Rare Alerts, Gathering, Fishing, Farming, Finder, Macro Editor, Camp Helper, Mage Travel, Shaman Totems, and more |

The [module list](docs/wiki/modules.md) describes every module and shows which ones start on, and the [feature showcase](docs/showcase/overview.md) goes into detail.

## Install

1. Download `EldoUI-<version>.zip` from the [releases page](https://github.com/Eldodeldo/EldoUI/releases).
2. Close the game and unzip the file into `World of Warcraft\_forever_\Interface\AddOns`. The WoW: Forever beta used the folder `_classic_beta_`; if you played the beta, install EldoUI again into `_forever_`.
3. Check that these folders sit directly in `AddOns`: `EldoUI`, `EldoUI_LootData`, `EldoUI_GuideData`, `EldoUI_LootSim`, `EldoUI_Emoji`, and `EldoUI_Locale_daDK`.
4. Start the game, make sure **EldoUI** is ticked in the AddOns list, and log in.

The five companion folders load only when you need them: the Loot Guide data, the guides, the gear simulator, the chat emoji, and the Danish texts.

### Updating

Close the game, delete the old EldoUI folders, and unzip the new version. Your settings live separately in the game's `WTF` folder. Keep a backup of that folder before updating. See [Updating](docs/wiki/updating.md) and [Starting with 0.7.1000](docs/wiki/updating-from-0-6.md).

## First start

The setup opens on your first login. Start with a preset pack (a whole UI in one click) or walk through the steps: UI scale, layout, look, accessibility, role, the addons you already use, modules, Blizzard's own UI, chat, game settings, other addons' profiles, convenience, and your keys and spells. Nothing changes until you click Apply or Finish, the last page puts back any part you change your mind about, and `/eui install` runs the setup again at any time.

New to EldoUI? Start with [Getting started](docs/wiki/getting-started.md).

## Commands

| Command | What it does |
|---|---|
| `/eui` | Open the config window |
| `/eui help` | Show every command in game |
| `/eui install` | Run the setup again |
| `/eui move` | Unlock frames to drag them; run it again to lock |
| `/eui layout <name>` | Apply a layout; `/eui layout` alone lists them, `/eui layout undo` puts back the last change |
| `/eui <module> on` or `off` | Turn a module on or off, for example `/eui nameplates off` |
| `/eui kb` | Keybind mode: hover a button and press a key |
| `/eui export` and `/eui import` | Share your setup as a string |
| `/eui data` | The Saved data page: copies from before each update, ready to put back |
| `/eui errors` | Show EldoUI's error log |

The [command reference](docs/wiki/commands.md) lists all of them.

## Compatibility

- **Game:** WoW: Forever (Interface 16001). EldoUI does not run on Classic Era or Retail.
- **Languages:** EldoUI's own texts are in English (US) and Danish: pick Dansk under General > EldoUI language and reload. The Loot Guide is also translated into German, French, Spanish, Brazilian Portuguese, Russian, Korean, and Chinese.
- **Other addons:** EldoUI works next to Details!, BigWigs, Deadly Boss Mods, Questie, RestedXP, Guidelime, HandyNotes, and Masque. For recognized addons, it offers ownership choices for supported jobs such as bags, bars, frames and chat: a whole module (Bags while Bagnon is loaded) or only the parts both do (selling gray items with Leatrix Plus). You pick who handles each job on the Other addons page, with `/eui addons`, or in the setup. See [Using EldoUI with other addons](docs/wiki/other-addons.md).

## Privacy and safety

EldoUI never connects to the internet and sends nothing to its author or to any website. It changes how the game looks and shows what the game already tells you; it never plays for you, and every chat line, invite, roll or purchase comes from your own click or key press. Some features exchange information with other players through addon messages. Examples include:

- **Version check** (on by default) tells guild and group members which EldoUI version you have, so you get one chat line when someone has a newer one. Never sent in combat, boss fights or PvP matches. Turn it off under Plugins > Notices.
- **Party Quests sync** (on by default) shares your quest progress with your group and shows theirs. Not in battlegrounds or arenas. Turn it off under Party Quests > Sync with group.

## Documentation

- [Getting started](docs/wiki/getting-started.md)
- [Updating](docs/wiki/updating.md) and [Starting with 0.7.1000](docs/wiki/updating-from-0-6.md)
- [Saved data](docs/wiki/saved-data.md)
- [Modules](docs/wiki/modules.md)
- [Layouts and presets](docs/wiki/layouts.md)
- [Eldostar](docs/wiki/eldostar.md)
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

Plugins add their own modules to EldoUI through the global `EldoUI` and get a settings page, a setup step, and the same look as the rest of the UI. See the [plugin guide](docs/PLUGINS.md).

## Credits

EldoUI is written from scratch for WoW: Forever, and it builds on the work of the WoW addon community:

- **Builds on** the embedded libraries LibStub, CallbackHandler-1.0, and LibActionButton-1.0; open-source code from What's Training?, Molinari, and Forever Journal; loot data from CMaNGOS classic-db; guides from the Polestar community guide project; and open fonts, sounds and emoji.
- **Inspired by** addons players already love, such as ElvUI, EllesmereUI, Plater, Details!, and Leatrix Plus, and by public community layout presets: seven of the eleven built-in layouts take their general idea from one.

Thank you to all of their authors. The full list, with every license, is in [Credits and third-party notices](THIRD_PARTY_NOTICES.md) and the [media credits](LICENSES/Media.md).

## License

Copyright 2026 Eldodeldo. EldoUI is licensed under the [Apache License, Version 2.0](LICENSE) (see also [NOTICE](NOTICE)).

Bundled libraries, adapted code, data, fonts, and sounds keep their own licenses. The `EldoUI_LootData` folder is licensed under GPL-3.0-or-later because its data comes from CMaNGOS classic-db, and the `EldoUI_GuideData` folder under GPL-3.0 because its guides come from Polestar.
