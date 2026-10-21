# Saved data

EldoUI keeps your settings, your journal and everything it remembers for you in the game's own saved files. It treats them like a guild bank: nothing leaves without you asking. Before an update changes anything, a copy is kept. A value EldoUI can't read is set aside, never deleted. And the **Saved data** page lets you put any of it back.

Open it with `/eui data`, or find **Saved data** in the EldoUI settings.

## Where your data is saved

An addon can't write files of its own. The game writes each addon's saved files when you log out, type `/reload`, or exit the game.

| File | What it holds |
|---|---|
| `WTF\Account\<account>\SavedVariables\EldoUI.lua` | Everything shared by your characters: profiles and settings, each character's journal and its backups, your characters' bags, bank, gold and mail for the Alts window, the instance log, Loot Guide lists, the error log, and the copies this page lists. |
| `WTF\Account\<account>\<realm>\<character>\SavedVariables\EldoUI.lua` | That character's chat message history. |

The `WTF` folder is in your game folder, next to `Interface`. Updating EldoUI replaces the addon folders only, never these files.

## The first login after an update

1. EldoUI reads which version wrote your saved data.
2. Before an update changes a profile, a journal or another saved part, it keeps a copy of that part as it was.
3. Then it brings the part up to date. Settings you never changed keep the value you saw, even when the default changed.
4. Your active profile is updated at once; your other profiles follow a few seconds later.
5. One chat line tells you what happened, and `/eui data` shows the details.

If an update step can't finish, the part stays as it was and the step runs again at your next login. If your saved data comes from a newer EldoUI (you went back to an older version), it is kept exactly as it is, including settings this version doesn't know.

## Backups

The **Backups** tab has four lists.

| List | What it holds |
|---|---|
| **Copies from before an update** | Each part as it was before an update changed it. |
| **Copies from before a restore** | What a part held just before you restored it, so one click undoes a restore. |
| **Journals of forgotten characters** | The journal of a character you forgot in the Alts window, backed up before it left. |
| **Kept as you put it back** | The parts you restored, which updates leave alone. |

- EldoUI keeps the newest copy of each part from before an update. A later update of the same part replaces it. If the same update runs again after a failed try, the first copy stays.
- The copies from before an update and from before a restore stay under 4 MB together, so your saved file stays quick to load. Past that, the oldest copies go first, and a chat line tells you. The newest copy of each journal from before an update is never let go.
- The journal of a forgotten character is kept until you put it back, whatever the size.
- Your journal and its dungeon runs also keep backups of their own on a schedule. See [Journal](journal.md#backups).

### Restoring a copy

Click **Restore** next to a copy, or type `/eui data restore <part> [<name>]`. It works out of combat.

- The part goes back exactly as it was before the update.
- What it held a moment ago is listed under **Copies from before a restore**. **Restore** there undoes your restore.
- Type `/reload` afterwards so every part of EldoUI reads it again.

Restoring a journal puts it back exactly as it was before the update. Moments you wrote since then leave the journal, but your journal as it was a moment ago is kept as a backup in My Adventure. To add back only what is missing, use **Restore a backup** with **Merge** in My Adventure instead.

### Journals of forgotten characters

When you forget a character in the Alts window, its journal is backed up first and listed here. **Restore** (or `/eui data restore journal <character>`) puts it back under its character. If that character has a journal again by then, the two are merged, so nothing from either is lost. The journal is on disk after your next logout or `/reload`.

### Kept as you put it back

A part you restored is held: updates leave it alone, so your restore sticks. It is listed under **Kept as you put it back**.

- **Let go** (or `/eui data follow <part> [<name>]`) lets it follow updates again. At your next login or `/reload` it is brought up to date, and the copy from before the update stays.
- A later EldoUI that brings a newer version of that part lets go by itself, after keeping a copy.

## Set aside, never deleted

Every saved part is checked the first time a session reads it.

- **Repaired**: small fixes that lose nothing. A number saved as text becomes a number, and a gap in a list closes up.
- **Set aside**: a value of the wrong kind (for example text where a list belongs) moves to the **Set aside** tab, and EldoUI carries on without it. Nothing is reset.

On the **Set aside** tab, **Put back** returns a value to its place. Whatever sits there now is set aside in turn, so nothing is lost. Type `/reload` afterwards.

The **Checks** tab lists what the checks found at this login, part by part, and which version of the saved data you have.

## Journals of another character

Each journal carries its character's own tag. If a journal saved under one of your character names belongs to someone else (for example a character you deleted and made again with the same name), EldoUI does not hand it to the new character. It keeps it under **Journals of another character** on the Set aside tab, however many there are, and starts a fresh journal.

## Leftover data

Saved tables from older versions that nothing in EldoUI reads any more are listed under **Leftover data** with their size. They stay until you click **Remove**. Remove asks first and can't be undone: it is the only button on the Saved data page that deletes anything.

## Privacy

- Your saved data stays on your PC. EldoUI has no server, and nothing on this page sends anything.
- A few group and guild features share small details with players in your group or guild when you turn them on, for example attunement progress or the recipes you know. Your journal, your backups and this page's copies are never part of that.
- Copies of your settings and journal live in the same saved file as the data itself. If you share that file, the copies go with it.

## Commands

| Command | What it does |
|---|---|
| `/eui data` | Opens the Saved data page and sums up what it holds. |
| `/eui data list` | Lists the copies from before an update, the journals of forgotten characters and the parts kept as you put them back, each with the command for it. |
| `/eui data restore <part> [<name>]` | Puts a copy back after you confirm, out of combat. Without a name, the newest copy of that part is used. Example: `/eui data restore profile Default`. |
| `/eui data follow <part> [<name>]` | Lets a part you restored follow updates again. |
| `/eui data help` | Shows these commands in chat. |

## FAQ

**Will an update wipe my settings or my journal?**
No. Before an update changes anything it keeps a copy, values it can't read are set aside instead of deleted, and nothing is reset.

**I updated and my setup looks wrong. How do I go back?**
Type `/eui data`, find the profile under **Copies from before an update**, click **Restore**, then `/reload`. The profile stays as you put it back until you choose **Let go**.

**I restored the wrong copy. Can I undo it?**
Yes. What the part held just before is under **Copies from before a restore**. Click **Restore** there, then `/reload`.

**I forgot a character in the Alts window by mistake. Is its journal gone?**
No. It is backed up first and listed under **Journals of forgotten characters**. Click **Restore** to put it back. Log in on that character again to fill its bags, bank and the rest anew.

**Why does the Backups tab say "No copies yet"?**
A copy is kept only when an update changes a part. If your saved data was already up to date, there was nothing to copy.

**The game crashed. Is my data gone?**
The game writes saved files when you log out, `/reload` or exit. A crash loses what changed since the last write, for every addon. Everything saved before that is still there.

**Can I go back to an older EldoUI?**
Yes. Your saved data is kept exactly as the newer version left it, including settings the older version doesn't know, so updating again later picks up where you were.

**How big can the copies get?**
The copies from before an update and from before a restore stay under 4 MB together. Past that the oldest go first, except the newest copy of each journal from before an update.

**How do I move my journal to another PC?**
Copy its backup code in My Adventure and paste it in there. See [Journal](journal.md#export-and-codes).
