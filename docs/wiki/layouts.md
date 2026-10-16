# Layouts and presets

EldoUI separates **where** things sit from **how** they look:

- a **layout preset** places every frame;
- **style presets** and the **art style** change looks only and never move anything;
- **movers** (`/eui move`) let you place any frame yourself on top of a layout.

## Layout presets

Seventeen layouts, all built on a 1440-unit-tall canvas (1440p). Pick one in the installer, on the Layouts page of `/eui`, or with `/eui layout <name>` (for example `/eui layout EldoClean`; `/eui layout` alone lists them). Eldo-Modern is the default.

| Layout | Idea |
|---|---|
| Eldo-Modern | Info bar on top, compact center, meters bottom right. |
| Eldo-Classic | Info bar at the bottom, stacked bar rows, guide and quests on the right. |
| Eldo-Clean | Minimal and clean: unit frames level with the utility cooldowns, everything else in its usual place. Inspired by MathaiusUI by Angelicus07. |
| Eldo-Cookies | Solo and leveling: low unit frames beside the top bar row, pet above the player, target of target above the target. Inspired by Cookies & Cream by .kreky. |
| Eldo-Zen | A quiet center: unit frames high, level with the resource bar, four stacked bar rows. Inspired by Zentyy Shaman Cleanest UI by Zentyy. |
| Eldo-Wide | Made for wide screens: unit frames well apart at cast bar height, pet beside the player, panels at the screen edges. Inspired by Wow Forever Preset by bigbluey. |
| Eldo-Blizz | Blizzard-style bottom block: unit frames sit right on the bar stack, pet and target of target above them. Inspired by Blizz-like Forever UI by figmentalnewton. |
| Eldo-Syntax | Dark and minimal: two bar rows, swing timers right under the character, unit frames beside the cooldowns. Inspired by SyntaxError UI by syntaxerror. |
| Eldo-Compact | Compact center built around the cooldowns: unit frames level with the essential row, buff bars above the target. Inspired by MattUI by dogobert. |
| Eldo-Joe | Wide center: cooldowns first, then resources and buffs, unit frames wide apart, side bars beside the bar stack. Inspired by JoeGaming v1.2 by joe_gaming1231. |
| Eldo-Heritage | Classic staggered unit frames, the target one row higher, party under the frames, bars along the bottom. Inspired by ratsiggy UI by 1fach. |
| Eldo-Hunter | Ranged and PvP: three bar blocks in a row, unit frames low and far apart for a clear center. Inspired by Hunter 1440p by l3nzu. |
| Eldo-Dark | Centered dark theme for melee: a breathing gap between resources and cooldowns, bars 1 and 3 side by side. Inspired by Rizka Forever Woyer by .rzk. |
| Eldo-Cozy | Cozy and close: the resource bar on top, unit frames right beside the character, bars in a small pyramid. Inspired by HedgeForever by mrhedge. |
| Eldo-Violet | Dark and minimal: all cooldowns in the center, wide-set unit frames at swing timer height, bars in one row along the bottom. Inspired by Midnight Lily by Lily TEAM. |
| Eldo-Plates | Tank and DPS: your target's details on its nameplate, the player frame inside the center column. Inspired by OnlyPlates by Trenchy TEAM. |
| Eldo-Zerby | Compact center: player and target close beside the resource bar, four slim bar rows under the character, party left of center. Inspired by ZerbyUI by Zerby. |

Eldo-Modern and Eldo-Classic are EldoUI's own. The other fifteen are built on EldoUI's own placement grid (zones, spacing and frame tracks on the 1440 canvas) with EldoUI's own accent colors; each takes only its general idea from a public community preset, credited above. No code, positions, colors or text are copied.

### Other screen sizes

- **Below 1440p**, EldoUI keeps the same 1440 canvas by default, so a layout looks the same on a 1080p screen, only smaller.
- **Ultrawide**: the Screen area page in `/eui` keeps EldoUI inside a centered area (16:9, 21:9 or your own width) while the game world fills the whole screen, so nothing ends up in the far corners.
- `/eui scale auto` goes back to the automatic scale; `/eui scale 0.64` sets your own.

## Moving frames

`/eui move` unlocks every EldoUI frame:

- drag a frame; it snaps to the grid and to other frames (hold Alt to place it freely);
- click a frame to nudge it by exact X and Y, or one pixel at a time;
- Shift-right-click a frame to put it back where the layout wants it.

`/eui move` again locks them. Your positions are saved per profile, on top of the layout. `/eui resetlayout` puts every frame back. EldoUI's frames also show in Blizzard's Edit Mode.

Blizzard windows (bags, character, mail and more) have their own mover: `/eui windows unlock`, then drag them; `/eui windows reset` puts them back.

## Style presets

Most modules have style presets: one click sets the look of that module (sizes, fonts, textures, colors), never its position. For example, Action Bars have One row, Two rows, Three rows, Four rows and a side bar, and Classic Blizzard; Unit Frames have Clean bars, Portraits, Minimal, Healer wide and Blizzard-like. Find them on each module's page and on the Style presets page in `/eui`, or in the installer's Styles step.

## Art style

The art style sets the frame look of every EldoUI panel and window:

| Art style | Look |
|---|---|
| Modern (flat) | Flat dark panels with a 1-pixel border and an accent line. |
| Blizzard | Dark panels with the game's rounded tooltip border. |
| Classic | Stone background with a gold-tinted border. |
| WoW Forever | Warm dark panels in the bronze frame line of the WoW: Forever action bars and micro menu, drawn from the game's own art. |

## Sharing a setup

- `/eui export` makes a share string of your whole profile (or `/eui export <module>` for one module); `/eui import` (or **Import and export > Import a string** in the options window) opens one paste box for every string: EldoUI, EllesmereUI, ElvUI and Edit Mode. It tells which kind you pasted and shows what it imports before anything changes. An EllesmereUI or ElvUI profile is rebuilt as an EldoUI layout (frame spots, bar shapes, sizes and which frames show and when): **Apply as a new layout** puts it on a new profile, **Change my current layout** puts it on the one you use; both can be undone.
- `/eui send <party|raid|guild|player>` offers your settings to others in game.
- Profiles: `/eui profile` lists them; see [Commands](commands.md#profiles-and-sharing).
