# Journal data reports

[My Adventure](my-adventure.md) suggests quests and dungeons that fit your level ("Next trips", the quest pages, "Where next" on Today). Those suggestions come from three layers:

1. **The quest data**: Classic values from the EldoUI_LootData folder.
2. **The Forever overlay**: what is new or different in WoW: Forever, shipped with EldoUI and updated with each release.
3. **What you saw**: the quests, dungeons, and zone levels the game showed you that the data does not know yet. It stays on your PC.

Players share what they saw with a **Journal data** issue, and it becomes part of the overlay. This page shows how, and what to do after a Forever patch.

## Report new content (players)

1. Keep **Remember new Forever content** on (My Adventure settings, Data tab; on by default). The journal then notes what quest dialogs, quest givers, and the map show you that the data does not know. Nothing else is read.
2. Play. The quest pages show what you saw right away.
3. When there is something to report, open the report in any of these ways:
   - `/eui journey report`
   - **Report new content** on the Data tab of My Adventure's settings
   - Ctrl-click the Journal button in the addon compartment (it says when there is something new)
4. A copy box opens with one `!EUJD1!` block. Select it all and copy it (Ctrl+A, Ctrl+C).
5. Open a new [Journal data issue](https://github.com/Eldodeldo/EldoUI/issues/new?template=journal-data.yml) and fill in the form:
   - **What kind of data**: the closest kind, or "Several of these" for a block from a long session.
   - **Export block**: paste the whole block.
   - **Where, and at which level**: for example "Goldshire, level 6".
   - **What did the game show?**: in your own words.
   - Tick **I saw this in the game myself**.
6. Submit. The form is read automatically and turned into a data update for review. If something is missing, a comment says what, and the issue gets the `needs-info` label; edit the issue and it is read again.

**A quest that is gone.** Pick "Quest gone" and list the quest IDs in "Quest, NPC, or map IDs". No block is needed.

**What a block holds.** Quests (title, level, giver and where it stands, who takes it, XP and money), dungeons (name, size, and levels), zone level ranges, and the client and data versions. Never your character's name. Nothing is sent from the game: you copy the block yourself.

**Only what you saw.** Never copy from Wowhead or from another addon's data. The bot refuses a form that names Wowhead.

## After a Forever patch

When a Forever patch changes quests or zones, check the data against the game. You need EldoUI_LootData installed.

1. `/eui journey check` asks the game about every quest of the data, a few each second and never in combat. `/eui journey check 30-45` checks only quests of levels 30 to 45. While it runs, `/eui journey check` tells you how far it is, and `/eui journey check stop` ends it early.
2. When it ends, a copy box lists the quests the game no longer knows and the zones whose level range in the game differs from EldoUI's.
3. File a "Quest gone" or "Zone level range" Journal data issue with those lines.

`/eui journey data` prints the versions and counts of the data, the overlay, and what you saw.

## What happens to a report

Every report is checked against the game before the data changes, and the corrected data ships with the next update.
