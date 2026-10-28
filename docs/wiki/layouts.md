# Layouts and presets

EldoUI separates **where** things sit from **how** they look:

- a **layout** places every frame;
- a **role** moves a few frames on top of it for the job you do in groups;
- **skins**, **style presets** and **preset packs** change the look and never move anything;
- **movers** (`/eui move`) let you place any frame yourself on top of all of it.

## Layout presets

All ten are built on EldoUI's own placement grid (zones, spacing and frame tracks on a canvas 1440 units tall). Pick one in the setup, on the Layouts page of `/eui`, on the Overview, or with `/eui layout <name>` (for example `/eui layout EldoZen`; `/eui layout` alone lists them). EldoUI Center is the default for new profiles.

| Layout | Key | Skin it brings | Idea |
|---|---|---|---|
| Vanilla Original | `EldoVanilla` | Vanilla Original | The familiar original layout: portraits in the top left corner, a round minimap top right, the action bars along the bottom with the chat beside them, and the world kept clear. |
| EldoUI Center | `EldoCenter` | WoW Forever | EldoUI's own default: one calm center. Player and target sit level with the cooldown row, the resource and cast bars stay in the column between them, and the action bars form one block at the bottom with a narrow wing on each side. |
| Modern Center | `EldoModern` | WoW Forever | Info bar on top, compact center, meters bottom right. |
| Blizzard Bottom Block | `EldoBlizz` | Blizzard | Blizzard-style bottom block: unit frames sit right on the bar stack, pet and target of target above them. |
| Portrait Staggered | `EldoHeritage` | Faction Heritage | Classic staggered unit frames with the target one row higher, party low on the left, three bar rows along the bottom with a short bar beside them. |
| Compact HUD | `EldoZen` | Minimal Modern | A quiet center: unit frames high, level with the resource bar, three stacked bar rows. |
| Widescreen Edges | `EldoWide` | WoW Forever | Made for wide screens: one long bar row along the bottom, unit frames well apart at cast bar height, pet beside the player, panels at the screen edges. |
| Close Combat | `EldoCozy` | Warcraft Parchment | Cozy and close: the resource bar on top, unit frames right beside the character, bars in a small pyramid. |
| Open Center | `EldoHunter` | Forged Metal | An open center for every class: three bar blocks in a row, unit frames low and far apart. |
| Nameplate Focus | `EldoPlates` | Forged Metal | Tank and DPS: your target's details on its nameplate, the player frame inside the center column. |

Each layout also suggests a style for each part of the UI and its own accent color. Picking a layout gives the same result wherever you pick it (the Layouts page, `/eui layout`, the Overview, a pack or the setup): the layout's skin, Blizzard windows and suggested styles, nameplates included.

- **Your own look stays yours.** If you picked a skin yourself, choosing a layout asks once whether to use the layout's look; **Keep my look** is the default.
- **Frames you dragged stay** where you put them when you change layouts, unless you tick **Put frames I dragged back in the layout's spots**.
- **Nothing happens twice.** Applying the layout and look you already use changes nothing.
- **Undo.** Every layout or pack change can be undone: press **Undo** on the alert after the change, or type `/eui layout undo`. Settings you changed yourself since then stay as you set them.

**Vanilla Original** with its own skin wears the game's own classic art: frames sized like the originals get the classic frame art, with the elite and rare dragons on the target; a one-row bar 1 sits on the classic stone tray with a gryphon at each end; the stance bar gets its classic stone; the micro menu and bag slots wear their classic buttons; and the round minimap gets the classic border, scaled with the map. The layout shows them as soon as you pick it.

### One picker

The Layouts page, the Overview and the move panel share one layout picker: the ten layouts first, then the legacy layouts one of your profiles still uses (**Legacy in use**), then **My layouts** (imported layouts and the copies EldoUI kept of your dragged frames). The Overview and move mode show your layout, role, skin and Blizzard windows at a glance.

### Legacy layouts

Layouts that left the list in 0.7.0000 stay in EldoUI as legacy layouts, unchanged: a profile that uses one keeps its screen until you pick another layout. A legacy layout shows in the picker only while one of your profiles uses it, together with the layout it is closest to, for example "Legacy: Eldo-Cookies (nearest: Portrait Staggered)". `/eui layout <name>` still applies one by its old name. [Updating from 0.6](updating-from-0-6.md#legacy-layouts) lists every legacy layout and its nearest layout.

## Roles

A role is not a layout. It is a small layer over any of the ten layouts for the job you do in groups, picked in the setup or on the Role page in `/eui`. Boss frames, boss mod bars and your cast bar never move by role.

| Role | What it changes |
|---|---|
| **Melee** | Frames stay where the layout puts them; party frames are a little more compact. |
| **Ranged** | Frames stay where the layout puts them; party frames are a little more compact, and the mana bar shows the five-second rule. |
| **Healer** | Party and raid frames move next to the center and grow, with dispel and boss debuff highlights, heal prediction and HoT squares. The spot is set for each layout, and frames in the way step aside: aura groups, the ping feed, combat text and the optional bars and panels. Raids that use the Mid or Large raid settings keep the larger healer frames too. **Healer group frames** on the Role page can put them at the bottom center instead, above your bars: the party as one row and a raid of up to ten as two rows, while a larger raid moves beside the center. Click-casting is offered as a choice. |
| **Tank** | Threat colors on nameplates and EldoUI's threat meter at its placed spot. Main tank frames show in raids. Nothing else moves. |

Every layout works with every role, without any setup of your own. The setup suggests Melee for Warriors and Rogues and Ranged for Hunters, Mages and Warlocks, and **Class details** adds a few settings for your class on top.

## Action bars and keys

Bars 1 and 2 always show. A layout may hide bar 3 and the bars after it, and their keys keep working.

- **Bar 3** shows nine buttons, in a shorter row or a 3x3 block, and holds what you use between pulls, such as buffs, resurrection and travel spells. Its buttons 10 to 12 keep their actions and your own keys. Widescreen Edges and Open Center keep all twelve, so bars 2 and 3 stay an even pair beside bar 1.
- **Hidden bars.** A bar the layout hides, or a bar from 3 up whose **Show on screen** switch you turn off on the Action Bars page, keeps every action and every key. It hides in combat and shows when you point at it out of combat: bar 3 as a small box next to your bags, bars 4 to 8 at the right edge of the screen. Turn off **Show on mouse over** to keep it out of sight altogether. The same rule, **Mouse over, out of combat**, can be picked for any bar.
- `/eui keys hidden` shows how buttons out of sight are kept; their keys work either way.

### Key sets

A key set puts keys on bars 1 to 3 in one go. Pick one in the setup's **Keys and spells** step, on the **Keybinds** page in `/eui`, or with `/eui kb <set>`. Each opens a preview of every key first, nothing changes until you press **Apply**, and **Undo** (or `/eui kb restore`) puts your old keys back.

| Key set | Command | Keys |
|---|---|---|
| Classic movement (recommended) | `/eui kb movement` | W and S move, A and D turn, Q and E strafe. Bar 1 on 1-5 R F T G Z X C, bar 2 with Shift, bar 3 with Ctrl. |
| A/D strafe | `/eui kb strafe` | W and S move, A and D strafe, and you turn with the mouse. Bar 1 on 1-5 R F E Q Z X C, bar 2 with Shift, bar 3 with Ctrl. |
| Number row | `/eui kb numbers` | Bar 1 on 1 to =, bar 2 with Shift, bar 3 with Ctrl. Movement keys stay as they are. |
| Side-button mouse | `/eui kb mouse` | For a mouse with 12 side buttons that send 1 to =: bar 1 on the side buttons, bar 2 on Shift and the side buttons, bar 3 around your hand. |
| Shifted hand | `/eui kb esdf` | Your hand rests one key to the right: E and D move, S and F strafe, with more keys around them. Bar 2 with Shift, bar 3 with Ctrl. |

- **Your key set belongs to your profile,** so it stays the same on every layout, pack and style preset. Your other characters on the profile get one offer to use the same keys, or get them on their own when you pick **Automatic**. A key you set yourself is never written over, and bars 4 to 8 keep the keys you give them.
- **Every keyboard.** The sets know US, UK, Nordic, German and French keyboards and use the keys in the same places on each. **Check my keyboard** (`/eui keys keyboard`) finds yours from three key presses.
- **Game shortcuts.** A shortcut a set takes gets the same new key in every set, such as Alt-R for reply. `/eui keys` lists where bags, map and the rest are.
- **Bar 3's keys 10 to 12** use your health potion, your healthstone, and your mana potion (a bandage for Warriors and Rogues) through the [Consumable Bar](../showcase/features/combat.md#consumable-bar). Until that module is on, these keys stay free; the preview turns it on with one click.
- When a bar pages on Shift or Ctrl, or your text style hides the keys on bars 1 to 3, EldoUI tells you after you apply a key set and fixes it in one click.
- **I manage my own keys** in the setup or on the Keybinds page leaves every key as it is. `/eui kb` alone is keybind mode: hover a button and press a key.

### Spells on their keys

Every spell of every class and role has one fixed button: the spells you press in a fight sit on the easy keys of bars 1 and 2, and bar 3 holds what you use between pulls. Nothing is ever cast for you, your own buttons and macros stay yours, and every change below happens out of combat and comes with an Undo.

- **New spells.** A spell you learn has its own button on bars 1 to 3, the same on every character of your class. EldoUI asks to put it there (**Ask me**), does it for you (**Automatic**), or leaves it (**Off**). `/eui spells` opens the keys and spells preview, and `/eui spells undo` takes the last new spells off again.
- **Spell ranks.** After you learn a rank, EldoUI offers to move your buttons to it, and nothing changes until you apply. **Upgrade spell ranks automatically**, an option you turn on yourself, moves bars 1 to 3 and the gamepad bars for you instead. Macros, spells on your keep list and buttons kept at a low rank never change. `/eui ranks` and `/eui rankcheck` list the lower ranks, and a macro that names a lower rank is marked in the macro editor with a one-click update.
- **Fill bars 4 and 5**, an option you turn on yourself, puts your out-of-combat class spells, such as teleports, tracking, poisons and pet care, on the empty buttons of bars 4 and 5. `/eui fillbars undo` takes the last fill off.
- **A new role.** After a role change, EldoUI offers to put the class spells of the new role on your bars: on empty buttons and on buttons where it placed a spell of your old role.
- **Hidden keys in the Cooldown Manager.** Its **Key text** shows the key of a spell on a button you can't see, such as on a hidden or shortened bar. It can also show the key on every icon, or on none.

These options are on the Action Bars page and in the setup's **Keys and spells** and **Convenience** steps.

## Moving frames

`/eui move` unlocks every EldoUI frame:

- drag a frame; it snaps to the grid and to other frames (hold Alt to place it freely);
- click a frame to nudge it by exact X and Y, or one pixel at a time;
- right-click a frame for its menu: hide or lock the box, reset its position, or open its options. On the action bars, the pet and stance bars, the micro menu and the bag bar the menu also has **Size** and **Spacing**, and the pet and stance bars can be laid out **Horizontal**, **Vertical** or as a **Grid**;
- Shift-right-click a frame to put it back where the layout wants it;
- **Find a frame** in the frames menu shows, selects and flashes any frame's box, and brings a frame that ended up off the screen back to the nearest edge.

`/eui move` again locks them. Your positions are saved per profile, on top of the layout. `/eui resetlayout` puts every frame back. EldoUI's frames also show in Blizzard's Edit Mode.

Blizzard windows (bags, character, mail and more) have their own mover: `/eui windows unlock`, then drag them; `/eui windows reset` puts them back.

### Other screen sizes

- **Below 1440p**, EldoUI keeps the same 1440 canvas by default, so a layout looks the same on a 1080p screen, only smaller.
- **Ultrawide**: the Screen area page in `/eui` keeps EldoUI inside a centered area (16:9, 21:9 or your own width) while the game world fills the whole screen, so nothing ends up in the far corners.
- `/eui scale auto` goes back to the automatic scale; `/eui scale 0.50` sets your own.
- **Which scale to pick:** Auto is the recommended scale, the one every layout is made for. A smaller scale is supported on a 1440p or larger screen: the layouts keep their room and the text gets smaller. A larger scale gives the layouts less room than they were made for, so frames can overlap. For bigger text, keep Auto and turn on **Large text** on the Accessibility page. The UI scale choice in the options and in the setup marks every value this way.
- **Other screen shapes:** The layouts are made for 16:9. A 16:10 screen is a little narrower at the same height, so every layout gives the boss frames, and in some layouts a few more frames, a spot of their own there: the bars, unit frames, boss frames and damage meter keep clear of each other. A few frames that show only now and then (timers, toasts, the durability figure) and boss mod windows can still overlap a neighbor there. An ultrawide screen (21:9) uses the 16:9 spots with more room at the sides.

## Skins

The skin frames every EldoUI panel and window, and Blizzard's windows when EldoUI may skin them. Pick one on the Appearance page, in the setup's Styles step, or let the layout bring its own.

| Skin | Look |
|---|---|
| Modern (flat) | Flat dark panels with a 1-pixel border and an accent line. |
| Minimal Modern | Flat charcoal panels with one fine hairline and square corners, the quietest skin. |
| Blizzard | Dark panels with the game's rounded tooltip border. |
| Classic | Stone background with a gold-tinted border. |
| WoW Forever | Warm dark panels in the bronze frame line of the WoW: Forever action bars and micro menu, drawn from the game's own art. |
| Vanilla Original | The game's own original frames: the classic player and target frames with the elite dragon, the gryphon-capped action bar and the round minimap border. Windows get carved gray stone with a warm brass double line. |
| Vanilla Refined | The classic look tidied up: satin graphite, a fine bronze double edge and softened corners, with thin portrait rings. |
| Warcraft Parchment | Dark oak panels in a leather binding with paper trims and stitched seams. |
| Forged Metal | Hammered iron with clipped steel rims, riveted corner plates and octagon portrait frames. |
| Portrait Classic | Polished slate with layered silver lips. |
| Faction Heritage | Your faction's materials in one shared frame, in Alliance, Horde or Neutral. |
| Arcane | Obsidian glass with faceted silver edges. |
| High contrast | Black panels with bright 2-pixel borders and no transparency, for low vision (also on the Accessibility page). |

Switching skins, profiles or themes shows the new look right away, without a reload.

## Style presets

Most modules have style presets: one click sets the look of that module (sizes, fonts, textures, colors), never its position. For example:

- **Unit Frames**: Clean bars, Portraits, Minimal, Healer wide, Blizzard-like, Classic frames and Boxed. Classic frames gives the player, target, target of target and pet frames the shape of the original frames, with a round portrait.
- **Party and Raid**: Vertical list, Healer grid, Wide bars, Blizzard-like, Minimal, Boxed and Raid leader.
- **Action Bars**: Standard, Clean, Macro names, Compact and Large.
- **Nameplates**: EldoUI, Twilight slim, Whisper, Beacon, Old road, Bastion and Headline.
- **Minimap**: Square, Large, Minimal, Clock only, Framed, Round and Button rail.

Find them on each module's page, on the Style presets page in `/eui`, or in the setup's Styles step. A unit frame graphics choice that does not fit your layout is grayed out, with the reason in its tooltip.

## Preset packs and complete looks

A preset pack is a whole UI in one click: a layout, a skin, a style for each part of the UI, a role, and the Blizzard UI and chat setup. Apply one from the setup's Welcome step or the Overview; it can be undone like any layout change.

| Pack | What you get |
|---|---|
| Modern | EldoUI's own look: the layout picked for your screen, clean unit frames and the layout's own skin. |
| Classic | Blizzard's shape in EldoUI's frames: portraits, the bars in a block at the bottom and macro names on the buttons. |
| Vanilla | The familiar original layout: portraits in the corners, a round minimap, one bar row along the bottom and Blizzard's own windows. |
| Healer | Big group tiles with heals on the way, unit frames close to the center and the Healer role with click-casting suggestions. |
| Minimal | A quiet screen: thin unit and group frames, no keybind text, a small minimap and a quiet info bar. |
| Structured | A tidy modern screen: everything under your character, quiet flat panels with a fine edge and EldoUI's helpers. |
| Focus | An open middle and a quiet screen: high frames, the quietest skin and only what you need to play. |
| Portrait Forge | Classic portraits in round medallions, the bars in a block at the bottom and EldoUI's helpers. |

Structured, Focus and Portrait Forge are complete looks: one layout, one skin and one UI amount each. The **UI amount** (Essential, Moderate or Full) sets how many of EldoUI's optional modules are on.

## Sharing a setup

- `/eui export` makes a share string of your whole profile (or `/eui export <module>` for one module); `/eui import` (or **Import and export > Import a string** in the options window) opens one paste box for every string: EldoUI, EllesmereUI, ElvUI and Edit Mode. It tells which kind you pasted and shows what it imports before anything changes. An EllesmereUI or ElvUI profile is rebuilt as an EldoUI layout (frame spots, bar shapes, sizes and which frames show and when): **Apply as a new layout** puts it on a new profile, **Change my current layout** puts it on the one you use; both can be undone.
- `/eui send <party|raid|guild|player>` offers your settings to others in game.
- Profiles: `/eui profile` lists them; see [Commands](commands.md#profiles-and-sharing).
