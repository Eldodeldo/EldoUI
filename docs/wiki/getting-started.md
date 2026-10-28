# Getting started

> Documentation for EldoUI **0.7.0002**. See [Current release](current-release.md) for this version's changes.

EldoUI is an AI-made, deeply modular UI for **WoW: Forever** (the game folder `_forever_`). It does not run on Classic Era or Retail.

## Install from a release zip

1. Download `EldoUI-<version>.zip` from the [GitHub releases](https://github.com/Eldodeldo/EldoUI/releases).
2. Close the game.
3. Unzip it into `World of Warcraft\_forever_\Interface\AddOns`. You get six folders, and all six must sit directly in `AddOns`:
   - `EldoUI`, the addon itself;
   - `EldoUI_LootData`, the data for the Loot Guide (loaded only when the Loot Guide needs it);
   - `EldoUI_GuideData`, the guides for the guide window (loaded only when the guide window needs them);
   - `EldoUI_LootSim`, the Loot Guide's gear simulator (loaded only when you press a sim button);
   - `EldoUI_Emoji`, the pictures for chat emoji (loaded only when chat emoji are on);
   - `EldoUI_Locale_daDK`, EldoUI's texts in Danish (loaded only when you pick Dansk as EldoUI's language).
4. Start the game. On the character screen, open **AddOns** and make sure **EldoUI** is ticked.

If you unzip into a folder of its own by mistake (`AddOns\EldoUI-<version>\EldoUI\...`), the game does not see EldoUI. Move the six folders up into `AddOns`.

Updating from 0.6? Read [Updating from 0.6](updating-from-0-6.md) first: your setup carries over, and that page shows where things moved.

## The setup

The setup opens on the first login of each character, and `/eui install` runs it again at any time. Every step is optional: **Skip** leaves that part as it is, and nothing changes until you click **Apply** on a step or **Finish**. A layout or UI scale you try is only a preview until then, and **Back** puts your old one back.

### Welcome

Pick the profile the setup writes into: the shared EldoUI profile as it is (on an alt, when another character set it up), a fresh EldoUI profile, or the one you use now.

Then go two ways:

- **A preset pack** is a whole UI in one click: a layout, a skin, a style for each part of the UI, a role, and the Blizzard UI and chat setup. **Apply** sets up every step with the pack and then shows your keys and spells; **Customize** walks through the steps with the pack's picks filled in. The packs are Modern, Classic, Vanilla, Healer, Minimal, Structured, Focus and Portrait Forge.
- **The steps**, one at a time:

| Step | What you pick |
|---|---|
| **UI scale** | How big the whole UI is. EldoUI is made for 1440p, and Auto (recommended) keeps that size on every screen. Every other value is marked as supported or not recommended. |
| **Layout** | One of the ten layouts (see [Layouts and presets](layouts.md)). Click one to preview it. |
| **Styles** | The skin for every window and panel, and one look per part of the UI. Choices depend on the layout and available space; check the preview before applying. |
| **Accessibility** | High contrast, large text and color-blind safe colors. Nothing is ticked unless you tick it, and General > Accessibility in `/eui` turns it off again and adds sound cues. |
| **Role** | Melee, Ranged, Healer or Tank: a small layer over your layout for the job you do in groups (see [Roles](layouts.md#roles)). Healers can also tick click-casting suggestions; nothing is bound unless you tick it. |
| **Addons you already use** | Shown only when EldoUI finds an addon that does the same job as part of EldoUI: keep that addon or let EldoUI do it (see [Using EldoUI with other addons](other-addons.md)). |
| **Modules** | Which EldoUI modules are on. A module that is off does nothing, and Blizzard's version stays. |
| **Blizzard UI** | Which of Blizzard's own frames and windows EldoUI may change. Anything EldoUI may not change stays as Blizzard made it. |
| **Chat** | Keep your chat windows, add EldoUI's chat tabs (whispers, loot, channels), or reset the chat windows first; a font size and class-colored names. |
| **Game settings** | A few of the game's own interface settings that fit EldoUI, such as locked action bars, cooldown numbers and detailed tooltips. Only what you tick changes, and **Blizzard default** in `/eui` puts your own values back. |
| **Other addons** | EldoUI's profiles for supported addons you use, such as Details! and BigWigs, imported with each addon's own import. Shown only for the addons EldoUI has a profile ready for. |
| **Convenience** | Every helper that acts for you, in one list: repairs, selling gray items, faster auto loot, the quest helpers, declining strangers' invites and more. **Recommended for me** ticks the ones that suit your class and level. Only what you leave ticked acts for you, and the same list is the **Conveniences** page under Modules in `/eui`. |
| **Keys and spells** | How you play: a key set for bars 1 to 3 or "I manage my own keys", your class spells and macros on empty buttons, spell rank upgrades, what happens with spells you learn later and on your other characters, your keyboard, and whether bars 1 to 3 show their keys. Each pack fills in its answers, and everything shows before it changes. A tick there turns on **Upgrade spell ranks automatically**, so later ranks move on their own, out of combat. Only this step's own **Apply** changes your bars: your own actions, macros, items and kept ranks stay, and one Undo puts it all back. The key set belongs to your profile, so it stays the same on every layout, and a key you set yourself is never written over. |

Plugins can add their own steps before the last page.

### The last page

The last page lists what **Finish** will do, with **Change** to go back to a step. After Finish it lists every change in groups, each with **Revert this**, and offers the reload.

Before the first change, EldoUI keeps a backup of the profile it writes into. **Undo the last setup** on the Welcome step (or `/eui install undo`) puts it back.

### On an alt

A new character on an account you already set up gets one short page instead of the whole setup: **Attach this character to** a profile you set up, with your class's profile listed first. It uses the profile as it is and brings only this character's own parts: chat tabs, game settings, click-casting and class spells, copied from the character you pick. A profile set up for another role can be copied for this one. The page shows what changes first, and Undo puts everything back. Open it again any time with `/eui attach` or from the Profiles page.

On an alt that uses a profile another character set up, the steps that change the whole profile (scale, layout, role, Blizzard UI and convenience) start on "keep", so clicking through can't undo your main's setup. Starting that profile fresh asks twice and names the characters that use it. Skipping the setup on a fresh profile still gives it the layout's sizes.

The setup waits while the game asks whether to skip the intro cinematic, and while another addon shows its own first-start window, and opens once you have answered.

## Find your way around

- `/eui` opens the config window. The search box finds any setting by its name, description or choices.
- The **Overview** page shows your layout, role, skin and Blizzard windows at a glance, with the preset packs and complete looks.
- `/eui move` unlocks the frames so you can drag them. `/eui move` again locks them.
- `/eui layout undo` puts back the last layout, pack or setup change.
- `/eui help` lists every command. See [Commands](commands.md).
- `/eui whatsnew` shows what changed in this version.
- Tour helps explain something new once, the first time you meet it. General > **Tour helps** turns them all off, **Show tour helps again** brings them back, and `/eui tour` lists them and shows one again.

## Language

EldoUI's own texts are in English (US) and Danish. Pick **Dansk** under General > **EldoUI language**, or in the language box on the setup's Welcome step, and reload. The choice holds for your whole account, and the game's own texts keep the game's language. Game words players say in English, such as quest, loot and raid, stay English in Danish too.

## Something went wrong?

`/eui errors` shows EldoUI's error log. The [FAQ](faq.md#how-do-i-report-a-problem) explains how to report a problem.
