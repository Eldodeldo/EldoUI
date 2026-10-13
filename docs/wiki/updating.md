# Updating

Your settings are saved in the game's `WTF` folder (`WTF\Account\<account>\SavedVariables\EldoUI.lua`), not in the addon folders, so updating never loses them.

## From a release zip

1. Close the game.
2. Delete the old `EldoUI`, `EldoUI_LootData`, `EldoUI_LootSim`, and `EldoUI_Emoji` folders in `Interface\AddOns`. (Unzipping over them works too, but deleting first makes sure no removed file stays behind.)
3. Unzip the new `EldoUI-<version>.zip` into `Interface\AddOns`.
4. Start the game. `/eui whatsnew` shows what changed.

Releases are listed on the [GitHub releases page](https://github.com/Eldodeldo/EldoUI/releases), and the [changelog](../../CHANGELOG.md) lists what changed in each version.

## After an update

- If a change needs a reload, EldoUI shows a banner with a Reload button.
- If a frame sits in a strange place after an update, `/eui resetlayout` puts every frame back to its layout position.
