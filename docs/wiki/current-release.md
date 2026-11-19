# Current release

<!-- eldoui:release-docs 0.7.3006 -->

EldoUI **0.7.3006**, 2026-11-19.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.3006) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.3006/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Info Bar

#### Fixed

- The Hit and Spell hit blocks count the hit rating on your gear, so they match the character sheet.

### Bags and loot

#### Fixed

- Every loot roll gets its roll bar at once, also while the item's details are still loading, so no roll is missed or shown in the game's own window instead.
- The game's own roll windows no longer reappear over the action bars after a loading screen while EldoUI's roll bars replace them.
- With the game's roll windows moved, each one opens directly on the roll spot and stays where it opened while other rolls start and end.
- Roll bars stay in the order their rolls started, so a new roll joins at the end instead of pushing the others down.
- The loot window closes with Escape, closing it ends the loot, an empty corpse or chest no longer leaves the loot open, and a leftover loot confirmation closes with the loot.
- Every item in the loot window shows, also one whose details the game keeps hidden, and a row from the last loot no longer disappears under a new item.
- EldoUI's bank window offers more bank space again: a button on its side bar buys the next bank tab, with its price and the game's own confirmation, also when the bag bar is off.
