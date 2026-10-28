# EldoUI

**An AI-made, deeply modular UI for WoW: Forever.** More than 90 modules you turn on and off one by one, ten layouts that place every frame for you, four roles on top of every layout, and one consistent look across all of it. Move anything with `/eui move`, change the look with skins and style presets, and share your setup as a string.

EldoUI stays within Blizzard's addon rules. It changes how the interface looks and where things sit, and shows only what the game gives addons. It never plays for you, and nothing acts without your click unless you turn it on.

## What you get

- **[Interface](features/interface.md)**: info bars, minimap, tooltip, maps, quest tracker, XP bars, micro menu, alerts and messages, and EldoUI skins for Blizzard's windows.
- **[Combat](features/combat.md)**: unit frames, action bars, nameplates, buffs and debuffs, player power, combat text, an encounter timeline, and Blizzard's combat displays and Cooldown Manager in the EldoUI look.
- **[Group](features/group.md)**: party and raid frames, click casting, raid tools, dungeon routes, raid loot lists, and ready check reports.
- **[Chat & Social](features/chat-social.md)**: chat with saved history and search, an instant messenger for whispers, player notes, and streamer mode.
- **[Items & Economy](features/items-economy.md)**: bags and bank across your characters, the Loot Guide, the My Adventure journal, upgrade arrows, auction house, merchant, mail, and trade.
- **[Quality of Life](features/quality-of-life.md)**: tweaks, waypoints, map notes, a rare scanner, gathering and fishing helpers, the Training window, and much more.

## The core

Every module shares the same core:

- **A guided setup** that sets up the whole UI from a preset pack in one click, or step by step: scale, layout, look, role, modules, chat, and your keys and spells. Nothing changes until you apply it, and every change can be reverted. See [Getting started](../wiki/getting-started.md).
- **Ten layouts** built for a 1440p canvas and applied in one click, from Vanilla Original to EldoUI Center, the default. Every layout or pack change can be undone. See [Layouts and presets](../wiki/layouts.md).
- **Four roles**: Melee, Ranged, Healer and Tank, a small layer over any layout. Healer brings the group frames to the center, Tank adds threat colors.
- **Keys and spells**: five key sets for bars 1 to 3 that know your keyboard and belong to your profile, new spells on their own button, and bars a layout hides that keep their keys. See [Action bars and keys](../wiki/layouts.md#action-bars-and-keys).
- **Tour helps** that explain something new once, the first time you meet it, and one short page that sets up a new character on a profile you already made.
- **Movers**: `/eui move` unlocks every EldoUI frame. Drag with grid snap, hold Alt to place freely, click a frame to nudge it by exact X and Y, and Shift-right-click to reset it. Frames you dragged stay where you put them when you change layouts. EldoUI's frames also appear in Blizzard's Edit Mode.
- **Skins and style presets** that change the look only, never positions: thirteen skins from Minimal Modern to Vanilla Original, which dresses the frames, bars and minimap in the game's own classic art.
- **One config window** (`/eui`) with a search that finds every setting, a mark on rows you changed (right-click resets one), a Recent changes list with undo, and a What's New page.
- **Profiles** per account or character, per talent group, and per content, and **share strings** to send a whole setup or one module to a friend.
- **Safe saved data**: a copy of your settings and journal before every update, and a Saved data page that puts any of it back.
- **Blizzard UI switches**: one switch per part of Blizzard's UI. Off leaves Blizzard's version alone.
- **Two languages**: EldoUI's own texts in English (US) or Danish.
- **A plugin API**, so other addons add their own modules with the same look. See [Plugins](../wiki/plugins.md).

## Built with AI assistance

EldoUI is designed and written from scratch with AI assistance, and tested for WoW: Forever. The open-source work it builds on and the work that inspired it are credited in [Credits and third-party notices](../../THIRD_PARTY_NOTICES.md).
