# Current release

<!-- eldoui:release-docs 0.7.3100 -->

EldoUI **0.7.3100**, 2026-11-21.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.3100) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.3100/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Setup and profiles

#### Fixed

- A character that moves to another ruleset is recognized at login: EldoUI asks once whether to bring over its settings, profile, Journal, bags and history, start fresh, or ask again later.

### Layouts and move mode

#### Fixed

- A full Consumable Bar no longer covers action bars, the stance bar or other boxes in any built-in layout, and in Compact HUD the incoming combat text no longer overlaps the reminders.

### Group frames

#### Fixed

- The instance counter uses WoW: Forever's limit of 10 new instances per hour, and raids for up to 20 players count toward it while 40-player raids do not. A limit you set yourself stays; the old default of 5 moves to 10 once.

### Action bars

#### Improved

- The key map gives your race's active abilities, such as Stoneform or Berserking, a key on buttons your class leaves free, and the keybind setup can place them. Classes with no free button keep them in the spellbook.

### Combat

#### Fixed

- In Warsong Gulch the Flag back bar runs 12 seconds after a capture, the time both flags take to return on WoW: Forever.

### Info Bar

#### New

- A new PvP rank block, and an optional PvP rank bar with the Status Bars, show your season rank and the Rank Points to the next one, or that you reached this week's cap. The tooltip adds the season total, the cap's rise, the season's end, the next rank reward and your kills.

### Bags and loot

#### New

- The Consumable Bar can show a button each for your cure against disease, bleeding and poison, picking the one that fits your level, and each can get a key. The Melee style turns them on.

#### Improved

- Item scores and upgrade arrows count the percent bonuses on WoW: Forever gear (hit, critical strike, haste, expertise, dodge, parry and block) in every client language, and the Loot Guide counts them for items the game has not loaded yet.

#### Fixed

- With the EldoUI skin on the game's combined bag, each slot keeps the game's art that shows which bag it comes from.

### Journal

#### New

- The Reputation page lists WoW: Forever's own factions, such as the Nightclaw Druids, Kirin Tor and The Watchers, with what each sells at every standing and the reputation still to go. Earthen Ring shows the standing where its reputation stops.

#### Improved

- Dungeon levels, "fits your level" and My Adventure's dungeon cards follow the levels the dungeon finder recommends whenever the game gives them, and the dungeon's tooltip says so.
- Rares and elites outside dungeons that the Loot Guide does not know yet, such as WoW: Forever's new ones, are now noted, and Report new content includes them so they can join the guide in a later version.
- The Attunements tab lists Barrow Deeps and Hyjal Summit with the day they open and what you can already get ready: level 60, the Brooch of the Wardens and each related reputation with its next reward. Their Journal pages say no attunement has been announced.
- The Onyxia's Lair attunement says that every raid member needs their own amulet.

#### Fixed

- When a help bubble is showing the first time you open the Loot Guide, its tour starts as soon as you close the bubble instead of on the next open.

### Leveling and quests

#### Fixed

- Eldostar's home, arrival and zone checks work on game clients in every language, so "make this inn your home" goals tick by themselves and steps meant for another zone show only where they should.

### Map and minimap

#### Improved

- Zone Info knows WoW: Forever's new zones (Riverglades, Shen'dralas, Mount Hyjal and Zephras Isle) and shows their level range and territory when the game gives none.
- Gathering knows WoW: Forever's Heavy Thorium vein in Mount Hyjal once you mine it: its pins and tooltip show the Mining 300 requirement, and the skill filter treats it like every other vein.
- Zone Info lists Krol'dok Stronghold as a dungeon of Riverglades, with its level range.

### Other addons

#### Improved

- More WoW: Forever addons are recognized. With a flight timer addon kept, EldoUI's flight bar stands back, and a resource bar addon takes over Class Resources' bars. Party and raid frame, loot browser, Hardcore and convenience addons get their own row on the Other addons page.

#### Fixed

- When the boss mod addon hides the quest tracker during a boss fight, EldoUI's Quest Tracker no longer shows it again mid-fight, and after the fight it follows your own visibility setting.

### Classes

#### New

- **Hunter:** The Training window's Pet abilities tab shows your pet's happiness with the damage it gives, whether loyalty is rising, its next loyalty rank, its experience and what its family eats. Beasts you could tame show what they eat in their tooltip.
