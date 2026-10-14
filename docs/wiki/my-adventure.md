# My Adventure

My Adventure is your character's journal. It is the first tab of the Journal window (the Loot Guide's window, `/lg`), called **My Adventure**, and it writes itself as you play: levels, places, dungeons, quests, finds, the people you traveled with, and your own goals and notes. It tells it back as a diary, a book from level 1 to 60, keepsake cards, and tips for where to go next.

- It needs the Loot Guide on. While My Adventure runs, the window's title reads "Journal" and the Loot Guide's dungeon tab reads "Dungeons".
- Switch it with `/eui adventure on` or `off`, or on the Modules page. `/eui adventure` opens its settings.
- It stays off while Forever Journal is loaded, so two journals never write the same thing. Its import still works then (see [Moving from Forever Journal](#moving-from-forever-journal)).

The journal only writes down what the game shows you. It never reads the combat log, never guesses kills or hidden numbers, and never does anything for you: every button opens a page, the map, or a waypoint.

## Opening it

| Where | What it does |
|---|---|
| `/eui journey` | Opens or closes My Adventure. `/eui journey <section>` opens a section, `/eui journey <text>` searches the journal. |
| `/lg` | Opens the Journal window on its start page: My Adventure, unless you picked another in the Loot Guide's settings. |
| Key bindings (Esc > Options > Keybindings > AddOns) | Open or close My Adventure, write a quick journal note, show or hide the journal tracker, open Next trips. |
| Addon compartment (the button by the minimap) | Left-click opens My Adventure, right-click writes a quick note, Shift-click opens Next trips, Ctrl-click reports new content when there is some. Its tooltip sums up your day. |
| Info Bar | The "Journal" datatext, with the same clicks. |
| Game menu (Esc) | The Journal button under EldoUI's button ("Journal button in the game menu", on by default). |
| Minimap | A Journal button, off by default ("Minimap button"). The Minimap module's button bin gathers it. |
| Quest menus | Right-click a quest in the quest log or the objective tracker: "Show in your journal", "Set as a goal", and "Write a note about it". |
| Tooltips | Item tooltips say when and where you found it; quest links say when you took and handed in the quest. |
| `/eui jot <text>` | Writes a note here and now. Without text it opens the quick note card. |

## The pages

The rail on the left groups the pages under Today, Story, and Atlas. "Open on" (settings, Journal tab) picks the page the tab opens on: Today, any page, or the last one you had open.

| Group | Page | What it shows |
|---|---|---|
| Today | Today | Where to go next, what is waiting for you, and what just happened. |
| Today | Next trips | Where to go next and why: dungeons with their quests, quests that fit your level, attunement steps, and zones to explore. |
| Today | Goals | Things you want to work towards. Their progress moves by itself as the game reports it. |
| Today | Notes | Notes that remember where and when you wrote them, and reminders that show when you get somewhere. |
| Story | Journey | Your story as it happened: chapters by level, day, or zone, with keepsakes, finds, and pinned notes. |
| Story | Book | Your story from level 1 to 60 as a book in chapters, in the tone you choose, with a cover for every part. |
| Story | Keepsakes | Your big moments as cards: first kills, epic finds, standings, mounts, and the moments you kept, with your firsts. |
| Story | Places | Every zone you visited with its corners, time, kills, and quests, and every dungeon with its runs. |
| Story | Quests | Every quest you handed in, with where, when, who gave it, and who came along; your quest log; the quests that left your log without a hand-in: abandoned, failed, or removed by the game (with where and when you took each one); and the quests the game remembers from before. |
| Story | Fellowship | The people you traveled with: time together and how it was spent, dungeons and quests together, and your notes on them. |
| Story | Story so far | Your character's story in a few lines, with the level river, your numbers, the eras, and ways to share it. |
| Atlas | Attunements | Attunements, keys, and dungeon quest chains, step by step, for each of your characters. |
| Atlas | Dungeons, Open World, Reputation | Open those tabs of the Journal window. |

**The character card.** Story so far has "Show card": a card with your name, class, level, time played, the level river, your numbers, and a few keepsakes, on a dimmed screen for your own screenshot. Companion names, your guild, and your realm are never on it. It also copies as text or Markdown.

**Search.** The Journal window's search box finds sections, places, goals, notes, and Journey moments ("VanCleef", "Frost Nova") under "Your journal".

## Moments and the tracker

- **Moments** are short cards in the alert lane for a new chapter (level), a new place, a first dungeon, a keepsake, a goal reached, rested time, and reminders. They wait while you are in combat. In a dungeon they are held, and one summary shows when you leave (or set "Moments in dungeons" to show them as they happen). Each moment plays one sound at most, and none when Fanfare already plays one for the same thing. The screenshot button on a card takes a screenshot only when you click it.
- **The journal tracker** lists your goals, reminders, and the next trip under your quests, in the quest tracker's column ("Keep it in the quest column"; with Questie it sits right under Questie's list). It has its own mover, "Journal Tracker", and hides when it has nothing to show.

## Styles

Six style presets set the look and how much the journal shows, never where anything sits. Pick one on the module's page.

| Style | What it sets |
|---|---|
| EldoUI | The Journal window's dark page and the EldoUI Book, the Storyteller detail with keepsakes, the tracker under your quests, and moments in the alert lane. |
| Storybook | Parchment pages with dark ink for the Book and the character card, told as a Chronicle. |
| Essentials | Levels, deaths, notes, goals, and keepsakes only, with short chapters, a small tracker, and fewer moments. |
| Chronicler | Everything, rare (blue) finds too, long chapters, every chapter open, and a taller tracker. |
| Compact | The Night ledger Book in smaller text, short chapters, and a slim tracker. |
| Quiet | No moments, no sounds, and no tracker. The journal still writes everything down, and reminders still show. |

With "Style follows the layout" on, applying a layout preset also gives the Book the look of the style that fits it (EldoUI, Storybook, or Compact). What the journal shows is kept.

## Settings

The module's page has seven tabs. Every option has its own description in the game.

- **Journal**: write the journal on or off, use the Characters and Instances records, the page it opens on, how much it shows (Essentials, Story, Chronicler, or your own ticks), finds from which quality, and the Journey's grouping.
- **Story**: the tone (Chronicle, Bard, or Ledger: the facts are the same in every tone), story length, how you are named, the Book look (Parchment, EldoUI, or Night ledger), and the reading size. Under Look, **Page look** puts the pages on the Journal window's dark panel or on paper (parchment with dark ink); the Book and the character card keep their Book look.
- **Where next**: how Next trips weighs dungeons, leveling, and collecting, raids on or off, briefs, the level-up page, and the prep checklist.
- **Moments and sounds**: which moments show, how long, in dungeons or after, their sounds, and Fanfare.
- **Tracker and buttons**: what the tracker lists and how tall it is, the quest column, the minimap and game menu buttons, and the key bindings.
- **Keeping it safe**: backups, restore, export, and clearing this character's journal.
- **Data**: what the journal reads from other modules, and new Forever content (see [Journal data reports](journal-data-reports.md)).

## Keeping it safe

An addon can't write files of its own, so the journal keeps dated backups inside its saved data.

- **Backups** are taken by themselves after you log in (every login, once a day, once a week, or only by hand) and before a restore, an import, or a clear. "Backups to keep" sets how many (1 to 10).
- **Restore** a backup with Merge (keeps everything since) or Replace (exactly as it was). Your journal is backed up first either way.
- **Backup code**: the whole journal as one `!EUJ1!` code in a copy box, to paste back on this PC or another (`/eui journey import code`, which also takes a Forever Journal `FJ1:` code). A pasted code is read as plain data only.
- **Export**: `/eui journey export markdown`, `html` (a printable page; print it to PDF in a browser), `text`, or `code`. Everything goes to a copy box. Nothing is ever sent from the game.
- **Clear this character's journal** takes a backup first.

## Moving from Forever Journal

`/eui journey import` reads Forever Journal's saved data while that addon is still enabled: every character's journal tagged with its owner, its backups, and optionally its settings. It never writes to Forever Journal's data, it backs up first, it can be undone, and running it twice adds nothing twice. Journals from before Forever Journal 1.3 carry no owner tag and are skipped, so a namesake's journal never lands on you. Then turn Forever Journal off in the AddOns list and `/reload`: EldoUI never turns another addon off.

## Where the data lives

- Each character's journal is in `EldoUIDB.journal["Name - Realm"]` (the account file, so alts can see each other), tagged with the character's GUID.
- Rows are packed and names are kept once. The journal keeps 8,000 rows and 2,000 quests; past that, small rows of old chapters fold into one summary per chapter. Levels, deaths, places, dungeons, goals, notes, and keepsakes are never folded.
- The budget is 1.5 MB per character. A typical character from 1 to 60 takes about 0.7 MB.

## Commands

| Command | What it does |
|---|---|
| `/eui journey` | Open or close My Adventure. |
| `/eui journey <section>` | Open a section: `today`, `next`, `goals`, `notes`, `journey`, `book`, `keepsakes`, `places`, `quests`, `fellowship`, `story`, `attune`. |
| `/eui journey <text>` | Search your journal. |
| `/eui journey data` | The journal data's versions and counts. |
| `/eui journey report` | Copy new Forever content for a journal-data issue. |
| `/eui journey check [from-to \| stop]` | After a Forever patch: check which quests of the data the game still knows. |
| `/eui journey export [markdown \| html \| text \| code]` | Export your journal to a copy box. |
| `/eui journey import [code]` | Import from Forever Journal, or paste a backup code. |
| `/eui jot [text]` | Write a quick note. |
| `/eui adventure [on \| off \| toggle \| <section>]` | Switch the module, open its settings, or open a section. |

## For plugin authors

Plugins can add pages, search results, moments, option rows, row kinds, and data sources to the journal: see [My Adventure API](my-adventure-api.md).

## Credits

Parts of the journal model, its event kinds, the goal and reminder rules, the backup merge, the pages' layouts and texts, and the parchment inks are adapted from [Forever Journal](https://www.curseforge.com/wow/addons/forever-journal) by Ugge Zen (MIT License). The list of files is in [THIRD_PARTY_NOTICES.md](../../THIRD_PARTY_NOTICES.md).
