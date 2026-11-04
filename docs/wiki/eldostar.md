# Eldostar

Eldostar is EldoUI's own guide window in **0.7.1000**. It follows community leveling, class quest, profession, reputation and collection guides. The guide texts are in English; the window and settings follow EldoUI's language choice.

## Start a guide

Open `/eui`, select **Eldostar**, and use **Guide > Guide on the guide spot** to choose Eldostar if another guide is selected.

1. Use `/eui eldostar show` for the guide window, or `/eui eldostar guides` for the guide list in the Journal under **My Adventure: Guides**.
2. If the list is unavailable, turn on **Loot Guide** and **My Adventure** in the module list. Choose Eldostar as the guide provider on Eldostar's settings page.
3. Use **For this character** to find matching guides, **All guides** to browse the full list, or search by name. Click a guide to start or continue it.

The guide title in the window opens the list again. At the level cap, Eldostar waits until you start a guide. The `EldoUI_GuideData` companion folder must be installed; it loads when Eldostar needs the guides. Guide availability depends on that data and your character.

## Follow the steps

- The window shows the step, its tip and its goals. Goals update from the information the game makes available, such as your quest log, bags, level, reputation and professions. Click to tick a goal the game cannot check.
- **Next** advances to the next step. **Skip** marks this step skipped. **Undo** takes back the last move, skip or tick.
- **Move on by itself** in the Guide tab advances a step when its goals are complete; turn it off to advance with Next.
- **Waypoint to the goal** uses the Waypoints module. A guide's coordinates take priority, with quest locations from the Loot Guide where available. A missing location cannot supply an arrow.

Eldostar never accepts or turns in a quest, buys an item or moves your character. You perform the actions in the guide.

## Pick who uses the guide spot

On Eldostar's settings page, **Guide > Guide on the guide spot** offers Automatic, Eldostar, RestedXP, Guidelime and Off. Automatic selects RestedXP when installed and enabled, otherwise Eldostar. Guidelime is an explicit choice. A selected external guide still needs its own addon and guides installed.

Only the chosen provider is placed in the layout's guide spot. This choice does not disable another addon; the page reports unavailable providers and any reload needed for positioning. See [Using EldoUI with other addons](other-addons.md).

## Window and progress

The **Window** tab offers Standard or Compact view, text size, tips, goals along the way, transparency, a window lock and visibility rules. Standard has a resize grip unless locked; **Reset the size** restores its size. `/eui eldostar show` reopens a closed window and `/eui eldostar hide` closes it.

Progress is saved per character and guide. **Stop the guide** keeps your place. Starting that guide again continues it; **Start the guide over** asks before clearing its progress. The Journal's guide list also offers Start over when you right-click a guide with progress.

Eldostar's route progress is separate from [My Adventure](my-adventure.md), which records your character's story, runs, quests and notes. See [Saved data](saved-data.md) before moving or replacing saved files.
