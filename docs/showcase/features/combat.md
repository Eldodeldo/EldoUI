# Combat

Your own frames, your bars and everything the game shows you in a fight. EldoUI dresses up and places what the game gives addons. It never computes hidden combat data and never plays for you.

[Back to the overview](../overview.md)

## Unit Frames

Player, target, focus, pet, target-of-target, boss, party pet and party target frames, plus switches for Blizzard's own unit frames and cast bar. Each frame has tabs for its bars, text tags, buffs and debuffs, cast bar and icons. Cast bars can hold a finished cast for a moment, flash, hide casts you cannot interrupt and mark important spells. Heal prediction and a fader are built in. Seven style presets include Classic frames, the shape of the original frames with a round portrait, and with the Vanilla Original skin, frames sized like the originals wear the game's own classic frame art, with the elite and rare dragons on the target. `/eui testframes` shows every frame with sample values so you can place and style them.

## Action Bars

Eight flat action bars plus pet, stance, vehicle, zone ability, totem and gamepad bars, each with its own size, fade and visibility rules. Cooldown numbers, proc glow and Masque support are built in. Keybind mode (`/eui kb`) lets you hover a button and press a key, and one-click keybind presets set up every bar. Buttons that still hold a lower spell rank light up while the spellbook is open; its Check ranks button (or `/eui rankcheck`) lists them, and `/eui ranks` moves them to the highest rank you know. After you learn a rank EldoUI offers the change, or, when you turn on Upgrade spell ranks automatically, moves bars 1 to 3 and the gamepad bars for you out of combat, with an Undo. Fill bars 4 and 5, when you turn it on, puts your out-of-combat class spells such as teleports, tracking and pet care on the empty buttons of bars 4 and 5. With the Vanilla Original skin, a one-row bar 1 sits on the classic stone tray with a gryphon at each end.

## Nameplates

Slim nameplates per unit type (enemies, friends, pets and more), with a cast bar, your debuffs, quest and elite icons, quest objective progress next to the quest icon, style filters and a target highlight. They wear your skin's frame edge and follow your unit frame graphics choice, and in big groups and cities each plate listens only to its own unit, so they stay light. Switches for Blizzard's nameplate parts and its nameplate settings come back as they were when you turn the module off.

## Buffs and Debuffs

Your buffs (right-click to cancel), debuffs, weapon enchants and boss mechanic auras in EldoUI frames, plus switches for Blizzard's buff frames. Filters, "yours first", blinking when an aura runs out and time bars are options.

## Class Resources

Health, power, combo points, druid mana and a GCD bar under your character, plus Blizzard's class resource frames. The five-second mana rule, color ranges, tick marks and extra bars are options, and totem timers have one owner here.

## Aura Groups

Your own rows of aura icons, each with its own mover: pick the spells, the unit and whether only yours count. The game shows each aura; EldoUI only places and dresses the icons.

## Combat HUD

Skins and places Blizzard's own combat displays: the damage meter, swing timer, loss of control, mirror and quest timers and death recap. Adds EldoUI's threat meter (`/eui threat`), a combat timer, a cursor ring with GCD and cast sweeps (`/eui cursor`) and a crosshair tinted by the game's own range check (`/eui crosshair`). `/eui hud` opens its settings.

## Cooldown Manager

Skins and places Blizzard's own Cooldown Manager: essential and utility cooldowns, buff icons and buff bars. Blizzard keeps tracking every cooldown; EldoUI only changes the look and the position. EldoUI's own rows add trinkets and mobility spells, and stand in when Blizzard's manager has no spells. Own groups (off by default) let you arrange those icons yourself: drag an icon into another group or onto empty screen in move mode, give one icon its own size, shape, border and up to three text labels, let icons slide when one hides, set a visibility rule per group, and keep a separate layout per talent group. `/eui cdm` opens it.

## Quickdraw

Hold a key for a ring, fan or grid of your own spells, items, macros, mounts and markers; let go on one to use it. Each menu has its own key binding. `/eui quickdraw` opens the menu editor.

## Shaman Totems

A totem bar with one button per element, a hover picker and Drop All, plus a cooldown bar for your shield, weapon imbues and Ankh. Save totem loadouts, share them as codes, see which party members your totems reach, and send a simple group plan. Totem timers kept with the totem bar move under or beside it when the cooldown rows fill the space above it. Every totem is cast by your own click.

## Pet Care

For hunters: a Feed Pet button next to the pet frame, and warnings when your pet is unhappy or your pet food runs low.

## Danger Alerts

Sound alarms when you stand in something harmful from a spell list, run low on breath, reach fatigue, or are attacked while away. Off by default.

## Enemy Spotter

A small list of hostile players seen on nameplates, with class color, level and how long ago you saw them. Off by default.

## Cast Bar Effects

Themed cast bars for EldoUI's cast bars and, when those are off, Blizzard's own: a color or gradient by spell school or class, a spark with a light trail, shine, border light, particles along the fill and flashes when a cast finishes, is interrupted or pushed back. Other units get one fixed theme each, so no spell is guessed. Particles keep to a budget and can be reduced or turned off in combat. `/eui castfx test` plays a test cast.

## Combat Text

EldoUI's own scrolling combat text, fed by the game's combat events: damage and healing taken, your hits on the target, notifications (procs, low health and mana, loot when loot toasts are off) and static lines, in movable scroll areas with their own animations, fonts and colors. Numbers can show on enemy nameplates (every hit on that enemy, labeled as such). It can hide or replace Blizzard's combat text, and steps back when MikScrollingBattleText, xCT+ or a similar addon is loaded. Six style presets. `/eui sct test` shows test lines; `/eui sct move` unlocks the areas.

## Cooldown Pulse

Shows a short pulse in the middle of the screen when one of your own spells or items is ready again, with an optional sound, spoken name and glow per entry. Spells with charges pulse when the first charge comes back. `/eui probe charges <spell>` prints each charge that comes back.

## Tracking Bars

One bar per spell under your cooldown rows: an aura's time left or stacks (in colored layers), a cooldown, or charges with a recharge strip. Colors can follow the time left, and the bars can match the width of a cooldown row or sit on their own mover.

## Consumable Bar

A small bar with one button each for food, drink, a health potion, a mana potion, a bandage and a healthstone. Each button holds the best item of its kind in your bags that your level can use (conjured food and water first, if you like), with the count and the cooldown. One click uses one item; nothing is used for you. Right-click a button to pick a specific item. Buttons change only out of combat. Six style presets (Standard, Caster, Melee, Compact, Vertical, Always all). Off by default; turn it on under Combat.

## Encounter Timeline

A small timeline right of center that shows the timers your boss mod publishes (Deadly Boss Mods or BigWigs) as icons sliding towards a now-marker, with warn and bad colors, lanes for timers close together, tick marks and a waiting stack. A big icon with a cooldown swipe shows the next timer. Pull, break and ready check timers get their own icons, and each kind has its own switch. An optional countdown sound (off by default) counts down the last seconds, and DBM's own bars can fade while the timeline shows. Test fights (Dungeon boss, Raid boss, Pull and break) show it without a boss. Six styles, horizontal or vertical, and a mover in every layout. The boss mod's own bars are left as they are. `/eui timeline` opens the options, `/eui timeline test raid` starts a test fight.

## Cast Tooltips and Mob Abilities

Point at the target or focus cast bar to see the spell's tooltip. NPC tooltips list the abilities you have seen that mob cast, and reputation turn-in items show where they go and the standing they give.

## Spell Efficiency

Spell tooltips get damage or healing per second, per mana, and the mana cost as a share of your pool, worked out only from the numbers the tooltip already shows.
