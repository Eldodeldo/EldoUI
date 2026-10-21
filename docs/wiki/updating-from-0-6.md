# Updating from 0.6

EldoUI 0.7.0000 changes how layouts, roles and saved settings fit together. Your setup carries over as it is: nothing is reset, nothing moves on its own, and a copy of everything is kept before the update touches it. This page shows what happens at your first login, what was renamed, and where things moved.

Install the new version as usual (see [Updating](updating.md)), then log in.

## Your first login

1. Before the update changes a profile, a journal or another saved part, EldoUI keeps a copy of it as it was.
2. Every profile is brought forward without removing anything. Settings you never changed keep the value you saw, even where the default changed. Your active profile is updated at once, the others a few seconds later.
3. One chat line tells you what happened.

`/eui data` opens the new **Saved data** page: it lists the copies, puts one back with **Restore**, and undoes a restore with one click. A saved value EldoUI can't read is set aside there instead of deleted. See [Saved data](saved-data.md).

## Layouts

The layout list is now the ten layouts on the [Layouts and presets](layouts.md) page. Your profile stays on the layout it used, and your dragged frames stay where you put them.

### Renamed layouts

Nine of the ten keep their place in the list under a clearer name. They keep their key, so `/eui layout` still finds them by the old name too.

| In 0.6 | Now | Key |
|---|---|---|
| Eldo-Vanilla | Vanilla Original | `EldoVanilla` |
| Eldo-Modern | Modern Center | `EldoModern` |
| Eldo-Blizz | Blizzard Bottom Block | `EldoBlizz` |
| Eldo-Heritage | Portrait Staggered | `EldoHeritage` |
| Eldo-Zen | Compact HUD | `EldoZen` |
| Eldo-Wide | Widescreen Edges | `EldoWide` |
| Eldo-Cozy | Close Combat | `EldoCozy` |
| Eldo-Hunter | Open Center | `EldoHunter` |
| Eldo-Plates | Nameplate Focus | `EldoPlates` |

**EldoUI Center** (`EldoCenter`) is new, and it is the default for new profiles. A profile that used the old default, Modern Center, keeps it.

### Legacy layouts

These layouts left the list. Each one stays in EldoUI as a legacy layout, exactly as it was, so a profile on it keeps its screen until you pick another layout.

| Legacy layout | Nearest layout |
|---|---|
| Eldo-Classic | Blizzard Bottom Block |
| Eldo-Clean | EldoUI Center |
| Eldo-Syntax | EldoUI Center |
| Eldo-Violet | EldoUI Center |
| Eldo-Joe | Modern Center |
| Eldo-Cookies | Portrait Staggered |
| Eldo-Compact | Compact HUD |
| Eldo-Zerby | Compact HUD |
| Eldo-Dark | Close Combat |
| Eldo-Vanilla Compact | Vanilla Original |
| Eldo-Vanilla Focus | Vanilla Original |

- The layout picker shows a legacy layout under **Legacy in use** while one of your profiles uses it, with its nearest layout, for example "Legacy: Eldo-Cookies (nearest: Portrait Staggered)". `/eui layout <name>` still applies one by its old name.
- If you had dragged frames on a legacy layout, EldoUI also keeps a copy of your screen, the legacy layout with your dragged positions, under **My layouts** as "*name* (my copy)". You can go back to it even after you pick one of the ten.
- To move on, pick the nearest layout (or any other) in the picker. Frames you dragged stay where you put them, unless you tick **Put frames I dragged back in the layout's spots**, and `/eui layout undo` puts the change back.

A profile that names a layout that is not installed says so once, places the frames by the default layout, and keeps your saved choice, so the layout comes back when it is installed again.

## Roles

The **Damage** role is now two roles, **Melee** and **Ranged**, next to Healer and Tank. A profile on Damage moves to your class's damage role by itself, and every frame stays where it was:

| Class | Becomes |
|---|---|
| Warrior, Rogue, Paladin, Shaman, Druid | Melee |
| Hunter, Mage, Warlock, Priest | Ranged |

An Elemental Shaman or a Balance Druid can pick Ranged on the Role page; Ranged adds the five-second rule to the mana bar. See [Roles](layouts.md#roles).

## What else moved or changed

- **Unit and party frames:** the style with the boxed 3D portrait and name bar is now called **Boxed**. Your pick stays.
- **Micro menu and bag bar:** a micro menu or bag bar you moved stays where you put it.
- **Keys and spells:** the setup has a new **Keys and spells** step. It changes nothing on your bars until you press its own Apply.
- **Action bars:** WoW: Forever has no extra action button, so its options and its key in keybind mode are gone. The zone ability keeps its own options and box in move mode.
- **Paladin:** the blessing reminder, the Blessing Plan and the ready check report count only the blessings that share the blessing slot on WoW: Forever. Salvation no longer counts as one, and Blessing of Sanctuary and Sanctity Aura are gone.
- **Shaman:** the totems and Earth Shield that WoW: Forever removed are gone from the pickers; a saved pick of one goes back to the first one you know.
- **Journal:** your journal carries over as it is, and its scheduled backups carry on. The first time your runs are read, the runs the instance log still has are copied into the journal with who was in them. See [Journal](journal.md#updating-from-eldoui-06).
- **Language:** EldoUI's own texts can now be shown in Danish, under General > EldoUI language.

## If something looks wrong

- Type `/eui data`, find the part under **Copies from before an update**, click **Restore**, then `/reload`. The part stays as you put it back until you choose **Let go**.
- `/eui layout undo` puts back the last layout or pack change.
- `/eui resetlayout` puts every frame back to its layout position.

Still stuck? The [FAQ](faq.md#how-do-i-report-a-problem) shows how to report it.
