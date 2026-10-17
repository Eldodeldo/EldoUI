# Getting started

EldoUI is an AI-made, deeply modular UI for **WoW: Forever** (the game folder `_classic_beta_`). It does not run on Classic Era or Retail.

## Install from a release zip

1. Download `EldoUI-<version>.zip` from the [GitHub releases](https://github.com/Eldodeldo/EldoUI/releases).
2. Close the game.
3. Unzip it into `World of Warcraft\_classic_beta_\Interface\AddOns`. You get four folders, and all four must sit directly in `AddOns`:
   - `EldoUI`, the addon itself;
   - `EldoUI_LootData`, the data for the Loot Guide (loaded only when the Loot Guide needs it);
   - `EldoUI_LootSim`, the Loot Guide's gear simulator (loaded only when you press a sim button);
   - `EldoUI_Emoji`, the pictures for chat emoji (loaded only when chat emoji are on).
4. Start the game. On the character screen, open **AddOns** and make sure **EldoUI** is ticked.

If you unzip into a folder of its own by mistake (`AddOns\EldoUI-0.6.0\EldoUI\...`), the game does not see EldoUI. Move the four folders up into `AddOns`.

## First login

The setup wizard opens on the first login of each character. It walks through:

1. **Welcome**: use the shared EldoUI profile as it is (on an alt, when another character set it up), a fresh EldoUI profile, or your current one.
2. **UI scale**: the 1440p canvas the layouts are made for, pixel perfect, or your own value.
3. **Layout**: pick one of the layout presets (see [Layouts and presets](layouts.md)).
4. **Styles**: style presets per module (looks only).
5. **Accessibility** (optional): high contrast, large text and color-blind safe colors. Nothing is ticked; a switch you tick can be turned off again in `/eui` > General > Accessibility, which also has sound cues.
6. **Role**: damage, healer or tank. Each moves a few frames to where that role wants them, on top of the layout.
7. **Addons you already use** (only when EldoUI finds one): for each job another addon does, keep that addon or let EldoUI do it. EldoUI is marked Recommended. Nothing changes before Finish, and Finish names every addon it turns off (see [Using EldoUI with other addons](other-addons.md)).
8. **Modules**: which EldoUI modules are on.
9. **Blizzard UI**: which parts of Blizzard's UI EldoUI may change.
10. **Chat**: keep your chat windows, add EldoUI's chat tabs, or reset the chat windows first; a font size and class-colored names.
11. **Game settings**: a few of the game's own interface settings that fit EldoUI (locked action bars, cooldown numbers, detailed tooltips and others). Only what you tick changes, and **Blizzard default** in `/eui` puts your own values back.
12. **Other addons**: set up supported addons (Details!, BigWigs and others) from EldoUI's profiles.
13. **Convenience**: auto repair, selling gray items and faster auto loot, only if you leave them ticked.

On an alt that uses a profile another character set up, the steps that change the whole profile start on "keep", so the alt can't undo your main's setup by clicking through. Skipping the setup on a fresh profile still gives it the layout's sizes.

`/eui install` runs it again at any time.

## Find your way around

- `/eui` opens the config window. The search box finds any setting by its name, description or choices.
- `/eui move` unlocks the frames so you can drag them. `/eui move` again locks them.
- `/eui help` lists every command. See [Commands](commands.md).
- `/eui whatsnew` shows what changed in this version.

## Something went wrong?

`/eui errors` shows EldoUI's error log. The [FAQ](faq.md#how-do-i-report-a-problem) explains how to report a problem.
