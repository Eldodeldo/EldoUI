# Journal

The journal is what [My Adventure](my-adventure.md) writes as you play. This page is about the journal's data: what it keeps, where it is saved, how it stays safe through updates, and how to back it up, move it or export it. For the pages and settings, see [My Adventure](my-adventure.md).

## What the journal keeps

Each character has a journal of its own:

- **Moments**: levels, places, dungeons, bosses, deaths, quests, finds, spells, professions, reputation, mounts, pets and flights, each with when and where.
- **Quests**: every quest you handed in, with where, when, who gave it and who came along, and quests that left your log without a hand-in.
- **Runs**: every dungeon and raid run, with who was in it (name, class, level, role and guild as the game showed them) and the loot rolls that ended while you were inside.
- **Companions**: the people you traveled with, and your notes on them.
- **Your own words**: goals, notes, reminders and notes on keepsakes.
- **Numbers**: time played, kills and deaths per level and zone, gold and experience earned.

It writes down only what the game shows you. It never reads the combat log, never guesses hidden numbers, and never does anything for you. Battlegrounds and arenas are not kept as runs.

## Where it is saved

Every journal is in your account's saved file, `WTF\Account\<account>\SavedVariables\EldoUI.lua`, so your other characters can read it in the Alts views. The game writes it when you log out, type `/reload`, or exit.

Each journal carries its character's own tag. A journal saved under a name that now belongs to another character (for example one you deleted and made again) is never handed to the new character: it is kept on the [Saved data](saved-data.md) page under **Journals of another character**.

**Size.** A journal has a budget of 1.5 MB per character. Moments are packed, and names are saved once.

- The journal keeps 8,000 moments. Past that, small moments of chapters two or more levels behind (spells, plain finds, flights and the like) fold into one summary per chapter, oldest first. Levels, deaths, places, dungeons, goals, notes and keepsakes never fold.
- The quest history keeps your newest 2,000 hand-ins, and the session list your newest 400 sessions.
- Runs have no cap: no run ever goes by itself. Each run keeps up to 40 loot drops and counts any more.

## Backups

An addon can't write files of its own, so the journal keeps dated backups inside its saved data (My Adventure > settings > **Keeping it safe**).

- **On a schedule**: 8 seconds after you log in, out of combat. Every login, once a day (the default), once a week, or only by hand.
- **By hand**: **Back up now**.
- **Before anything big**: before a restore, an import, and before an EldoUI update changes the journal.
- **Backups to keep**: 1 to 10 (3 by default). The oldest goes when a new one would pass the number. The newest copy from before an update has a slot of its own, so scheduled backups never push it out.

Your **runs** keep their own backups: the newest two, taken before a restore, an import, and before an update changes them. The newest copy from before an update is always kept as well. Restore them with **Restore your runs**.

A long journal, or years of runs, is backed up a little at a time while you play, and the work waits while you are in combat, so a backup never holds up your login. A copy from before an update is listed at once. While it is still being written, its code can't be copied yet, and a copy of your runs can't be restored yet.

A backup is on disk after your next logout or `/reload`.

### Restoring: Merge or Replace

Pick a backup with **Restore a backup** (or **Restore your runs**), then:

- **Merge** adds everything in the backup that your journal is missing and keeps everything since. Nothing from either is lost, and nothing is added twice.
- **Replace** puts the journal back exactly as it was then.

Your journal as it is now is backed up first either way.

## Updating from EldoUI 0.6

- Your journal already has the shape this version saves, so the update leaves it as it is, and its scheduled backups carry on.
- The first time your runs are read, the runs the instance log still has are copied into your journal with who was in them. From then on every run you finish is added as it closes.
- Instance log runs keep every raid member.
- If a future update changes the journal, a backup is taken first and listed on the [Saved data](saved-data.md) page.

## Repair, never reset

The first time a session reads a journal, EldoUI checks it:

- A number saved as text becomes a number, and a gap in a list closes up.
- A value of the wrong kind is set aside on the [Saved data](saved-data.md) page, where **Put back** returns it. The rest of the journal loads as usual.
- Anything the check doesn't know is kept as it is.

## Deleting things

Only you delete things, and you can change your mind:

- Deleting a moment, a goal, a note, a run, or a name from your runs asks first, and goes to the journal's trash for 7 days. **Undo** puts it back exactly.
- **Forgetting a character** in the Alts window backs up that character's journal first, then removes it from EldoUI. The [Saved data](saved-data.md#journals-of-forgotten-characters) page lists it under **Journals of forgotten characters**, and **Restore** puts it back.

## Export and codes

All of these go to a copy box: press Ctrl+C and paste them wherever you like. Nothing is sent from the game.

| Option | What you get |
|---|---|
| **Copy a backup code** | The whole journal as one `!EUJ1!` code: moments, quests, goals, notes and companions. Paste it back with **Paste a journal code** on this PC or another. |
| **Copy a runs code** | Your runs as one `!EUJR1!` code, with their members and loot rolls. Paste it back with **Paste a runs code**. |
| **Export as Markdown** | The journal as a readable document by chapter, with goals, notes, quests and runs. |
| **Export a printable page** | The journal as a web page (HTML). Save it as a `.html` file, open it in a browser and print it to PDF. |
| **Export as plain text** | The journal as plain text, by chapter. |

`/eui journey export markdown`, `html`, `text` or `code` does the same from chat. A pasted code is read as plain data only, and you see what it holds before anything changes.

## Moving from Forever Journal

**Import from Forever Journal** (or `/eui journey import`) brings every Forever Journal journal into My Adventure while that addon is still enabled. It only reads Forever Journal's data, merges instead of wiping, backs up first, and **Undo the import** puts every touched journal back. Running it twice adds nothing twice. A Forever Journal `FJ1:` code works with **Paste a journal code** too. See [My Adventure](my-adventure.md#moving-from-forever-journal).

## Privacy

- Your journal stays on your PC. Nothing in the journal is ever sent from the game: there is no button that sends it, and it can't be shared through addon messages.
- Your journal and runs remember the people you grouped with: names, class, level, role and guild as the game showed them, and their loot rolls. **Delete** on a run or **Forget this name** removes someone, with Undo for 7 days.
- **The Markdown, printable page and plain text exports leave companion names out.** They list how many were with you instead.
- **Backup codes and runs codes hold everything**, companion names included, so you can restore them in full. Share them only with people you trust.
- The printable page loads its fonts from Google Fonts when you open it in a browser.
- **Remember new Forever content** (settings, Data tab) notes quests, dungeons and zone levels the game shows you that the quest data doesn't know yet. **Report new content** puts them in a copy box; nothing is sent.

## FAQ

**Will updating EldoUI cost me my journal?**
No. Your journal is never reset. If an update changes it, a backup is taken first, and what a check can't read is set aside, not deleted.

**I made a mistake. How do I get yesterday's journal back?**
My Adventure > settings > **Keeping it safe** > **Restore a backup**. Pick the backup, then Merge to add back what is missing, or Replace to go back exactly. Your journal as it is now is backed up first.

**Can I keep my journal when I change PCs or reinstall the game?**
Yes. Copy the backup code and the runs code and keep them somewhere safe, then paste them in on the new PC. Copying your `WTF` folder works too.

**I deleted and remade my character. Where is the old journal?**
It is kept on the Saved data page under **Journals of another character**. The new character starts a fresh journal, so two stories never mix.

**I forgot a character in the Alts window. Can I get its journal back?**
Yes. Its journal was backed up first. Open the Saved data page (`/eui data`) and click **Restore** under **Journals of forgotten characters**.

**Why are some of my oldest small moments folded into a summary?**
A journal keeps 8,000 moments. Past that, small moments from older chapters fold into one summary per chapter so the journal stays light. Levels, deaths, places, dungeons, goals, notes and keepsakes never fold.

**Does the journal slow the game down?**
It is built not to. Long run lists open one page of 100 runs at a time, a journal with years of runs opens as fast as a new one, and its backups are written a little at a time.

**Does anyone else see my journal?**
No. Nothing in it leaves your PC unless you copy a code or an export yourself.
