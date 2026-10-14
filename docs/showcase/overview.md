# EldoUI

**An AI-made, deeply modular UI for WoW: Forever.** More than 90 modules you turn on and off one by one, 17 layout presets that place every frame for you, and one consistent look across all of it. Move anything with `/eui move`, change the look with style presets, and share your setup as a string.

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

- **One config window** (`/eui`) with a search that finds every setting, a mark on rows you changed (right-click resets one), a Recent changes list with undo, and a What's New page.
- **17 layout presets** built for a 1440p canvas and applied in one click. See [Layouts and presets](../wiki/layouts.md).
- **Movers**: `/eui move` unlocks every EldoUI frame. Drag with grid snap, hold Alt to place freely, click a frame to nudge it by exact X and Y, and Shift-right-click to reset it. EldoUI's frames also appear in Blizzard's Edit Mode.
- **Style presets and art styles** that change the look only, never positions.
- **Profiles** per account or character, per talent group, and per content, and **share strings** to send a whole setup or one module to a friend.
- **Blizzard UI switches**: one switch per part of Blizzard's UI. Off leaves Blizzard's version alone.
- **A plugin API**, so other addons add their own modules with the same look. See [Plugins](../wiki/plugins.md).

> Screenshot coming soon: the EldoUI config window with the sidebar and a module page open.

> Screenshot coming soon: `/eui move` with the grid and the movers shown in the Eldo-Modern layout.

## Built with AI assistance

EldoUI is designed and written with AI assistance and tested for WoW: Forever. Many features were inspired by well-loved addons from the WoW community, and the open-source projects EldoUI builds on are credited in [Credits and third-party notices](../../THIRD_PARTY_NOTICES.md).
