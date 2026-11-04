# Updating

For the **0.7.1000** interface and setup, start with [Getting started](getting-started.md). Check the [releases page](https://github.com/Eldodeldo/EldoUI/releases) for published downloads and [Current release](current-release.md) for the release-note reference.

Your settings are saved in the game's `WTF` folder (`WTF\Account\<account>\SavedVariables\EldoUI.lua`), not in the addon folders. Keep a copy of that folder before updating.

Version 0.7.1000 starts a fresh EldoUI profile. Earlier EldoUI profiles and presets are not supported. Updates from 0.7.1000 onward preserve supported settings; choose among the eleven presets on the [Layouts page](layouts.md).

## From a release zip

1. Close the game.
2. Delete the old `EldoUI`, `EldoUI_LootData`, `EldoUI_GuideData`, `EldoUI_LootSim`, `EldoUI_Emoji`, and `EldoUI_Locale_daDK` folders in `Interface\AddOns`. (Unzipping over them works too, but deleting first makes sure no removed file stays behind.)
3. Unzip the new `EldoUI-<version>.zip` into `Interface\AddOns`.
4. Start the game. `/eui whatsnew` shows what changed.

Releases are listed on the [GitHub releases page](https://github.com/Eldodeldo/EldoUI/releases), and the [changelog](../../CHANGELOG.md) lists what changed in each version.

## After an update

- Before an update changes your settings or your journal, EldoUI keeps a copy. One chat line tells you what changed, and `/eui data` opens the [Saved data](saved-data.md) page, where **Restore** puts a copy back.
- If a change needs a reload, EldoUI shows a banner with a Reload button.
- If a frame sits in a strange place after an update, `/eui resetlayout` puts every frame back to its layout position.
