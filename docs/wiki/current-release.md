# Current release

<!-- eldoui:release-docs 0.7.0003 -->

EldoUI **0.7.0003**, 2026-10-28.

[Download this version](https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0003) · [All changes](https://github.com/Eldodeldo/EldoUI/blob/v0.7.0003/CHANGELOG.md) · [Updating](updating.md)

These notes describe this version. Migration guides keep the version numbers of the updates they explain.

### Highlights
- Your key set now belongs to your profile and knows US, UK, Nordic, German and French keyboards, and new spells land on their own key on bars 1 to 3.
- Tour helps explain new parts of EldoUI the first time you meet them, and a new character on an account you already set up gets one short page instead of the whole setup.
- Eldostar, EldoUI's own leveling guide, brings over 200 community guides for WoW: Forever in a window on your layout, with a waypoint to the next goal.
- My Adventure has a Guides page where you start, follow and search the leveling guides.
- The Journal can group a boss's loot by kind and shows a branching dungeon quest chain as a flowchart.
- On a 16:10 screen the layouts give the boss frames, the boss mod windows, the party pets and many more frames a spot of their own.
- The UI scale choice shows which scales the layouts are made for, with Auto recommended.
- Switching style presets keeps your layout tidy, and a damaged saved settings file no longer stops EldoUI from loading.

### New
- **Setup and layouts:** A new character on an account you already set up gets one short page instead of the whole setup: it uses one of your profiles as it is, with its own chat tabs, game settings, click-casting and class spells.
- **Setup and layouts:** The alt page lists your class's profile first, can copy a profile set up for another role, and Undo puts everything back. Open it any time with /eui attach or from the Profiles page.
- **Action bars:** New spells land on their key: a spell you learn has its own button on bars 1 to 3, the same on every character of your class. EldoUI offers to put it there, or does it for you when you pick Automatically, on empty buttons only and with an Undo.
- **Action bars:** Upgrade spell ranks automatically, an option you turn on yourself: new ranks move onto bars 1 to 3 and the gamepad bars out of combat, with a chat line and an Undo. Macros, spells on your keep list and buttons kept at a low rank never change.
- **Action bars:** Fill bars 4 and 5, an option you turn on yourself: out-of-combat spells such as teleports, tracking, poisons and pet care go on the empty buttons of bars 4 and 5. Your own buttons stay, a spell you learn later joins them, and Undo takes them off.
- **Talents and spells:** A macro that names a lower spell rank, such as Frostbolt(Rank 3) after you learn Rank 4, is marked in the macro editor and the rank check. One click on Update to Rank 4 changes only the rank number, out of combat, and Undo puts it back.
- **General:** Eldostar is EldoUI's own leveling guide: over 200 community guides for WoW: Forever, step by step in a window on your layout's guide spot. Goals tick from your quest log, bags, level, reputation and professions, and a waypoint points to the next goal.
- **Journal:** My Adventure has a Guides page where you start a leveling guide for your character, see the one you are on and the one up next, and search every guide. At the level cap, Eldostar shows nothing until you start a guide there.
- **Setup and layouts:** The setup's Other addons step and Eldostar's options let you pick the one leveling guide that takes the guide spot: Automatic, Eldostar, RestedXP or Off. EldoUI never turns the other guide addon off.
- **Journal:** A boss's loot can be grouped by kind: quest items, weapons, armor, accessories and everything else, each with the most likely drop first. The Journal remembers whether you sort by chance or by kind.
- **Journal:** A dungeon quest chain that splits into several paths shows as a flowchart in the quest details: every quest is a box with your progress, joined by lines to the quests that follow it. Switch to the step list at any time, and the Journal keeps your choice.
- **Options:** The Other addons page has a new list, Also done by EldoUI: addons that run fine next to EldoUI but do a job EldoUI already does, in full or in part. For an addon whose whole job EldoUI does, one click turns it off for this character.
- **Group frames:** With the Healer role, the Role page can put your group frames at the bottom center, above your bars: the party as one row and a raid of up to ten as two rows. A larger raid moves beside the center on its own.
- **General:** Tour helps explain something new the first time you meet it: move mode, the Layouts and Blizzard UI pages, your keys after you apply a key set and the chat tabs the setup made. Each one shows once, and the Tour helps switch on the General options page turns them all off.
- **General:** More parts explain themselves once with a tour help: the bag window, the vendor list, Open all in the mailbox, the auction house tabs, healer click-casting, fishing mode, the minimap button rail, styles, keybind mode, profile rules, the guide window and Edit Mode.
- **Setup and layouts:** When a layout keeps an action bar out of sight, a tour help draws the bar where it sits and tells you its keys still work, naming the long cooldowns on it. Keep it hidden keeps it out of sight on mouse-over too.
- **Setup and layouts:** A layout whose bars show on mouse-over says so once, with a button to show them all the time, and after the setup a short help shows where to change your UI later.
- **Setup and layouts:** The setup's Convenience step lists every helper that acts for you, from repairs to the quest helpers, and "Recommended for me" ticks the ones that suit your class and level. The same list is the new Conveniences page under Modules.
- **Action bars:** Two new key sets: Side-button mouse puts bar 1 on a mouse with 12 side buttons, and Shifted hand rests your hand one key to the right for more keys around it.
- **Action bars:** The key sets know US, UK, Nordic, German and French keyboards and use the keys in the same places on each. Check my keyboard finds yours from three key presses.
- **Action bars:** A game shortcut a key set takes gets the same new key in every set, such as Alt-R for reply, and the game keys list (`/eui keys`) shows where bags, map and the rest are. Bar 3's last three keys use the Consumable Bar: potion, healthstone, and mana potion or bandage.
- **Action bars:** A new visibility rule, "Mouse over, out of combat", hides a bar in combat and shows it when you point at it outside a fight. Each bar from 3 up has a Show on screen switch that hides it this way, keys still working; turn off Show on mouse over to keep it out of sight altogether.
- **Action bars:** Your key set belongs to your profile now, so it stays the same on every layout, pack and style preset. Your other characters on the profile get one offer to use the same keys, or get them by themselves when you choose Automatic, and keys you set yourself are never written over.
- **Setup and layouts:** The Keys and spells step asks how you play: a key set or "I manage my own keys", what happens with spells you learn later and on your other characters, and whether bars 1 to 3 show their keys. Each pack fills in its answers, and nothing changes until you press Apply.
- **Action bars:** After a role change, EldoUI offers to put the class spells of your new role on your bars, only on empty buttons and on buttons where it placed a spell of your old role, with Undo.

### Improved
- **Action bars:** Bar 3 now shows nine buttons, in a shorter row or a 3x3 block, and keeps the actions and your own keys on its last three. Widescreen Edges and Open Center keep all twelve, so bars 2 and 3 stay an even pair beside bar 1.
- **Setup and layouts:** The Vanilla Original layout now offers the Large action bar style too; your bags open on top of the bars.
- **Setup and layouts:** Switching between style presets keeps your layout tidy: going back to a style puts every frame back exactly as that style placed it, and a style no longer keeps settings left over from the one picked before it.
- **Setup and layouts:** The Blizzard-like group frames can now be picked in the Portrait Staggered and Nameplate Focus layouts, and the Healer group frames in Nameplate Focus.
- **Setup and layouts:** On a 16:10 screen the boss frames, boss mod windows, party pets and targets, vehicle seat, pet and bag bars, Battle.net toasts, red error text and combat text get spots of their own, clear of the chat, the bars and the damage meter.
- **Setup and layouts:** Style presets and the setup now say what a style does to your layout: a style that makes a frame bigger moves its neighbors to make room, and one that doesn't fit is grayed out.
- **Map and minimap:** The minimap styles say when they can't show yet: while the game's own minimap is in use, Style presets and the setup tell you how to turn on EldoUI's minimap.
- **Map and minimap:** With a larger minimap style, the buff and debuff rows move out with the map and keep their distance to it, and on a round map the Split Timer and the quest list keep clear of the map's ring.
- **Setup and layouts:** In the EldoUI Center and Nameplate Focus layouts the experience bar is now as long as action bar 1, so it no longer reaches past the side bars when they are empty or hidden. A bar length you picked yourself stays as it is.
- **General:** The UI scale choice in the options and in the setup shows which scales the layouts are made for: Auto is recommended, and every other value is marked as supported or not recommended, with a short reason.
- **General:** EldoUI recognizes many more addons that do one of its jobs. Nameplate, buff, loot window, tooltip, chat, waypoint and world map addons now make EldoUI's own version stand back, so the two never draw the same thing twice, and you pick who handles each job on the Other addons page.
- **General:** In move mode with test frames, an empty action bar, buff or debuff row, quest tracker, cooldown row or swing timer shows a sample in your own sizes, colors and text, starting on the side it grows from, so you see the frame the way it will look.
- **Journal:** The Journal's tours follow the Tour helps switch, and Show tour helps again on the General options page brings them back too.
- **Action bars:** The offer to move your buttons to a new spell rank is now on for everyone and also checks once at login. It only asks, and nothing changes until you apply. It steps aside while another addon moves your spell ranks.
- **Action bars:** The spell rank check also covers the gamepad bars and finds a lower rank even where the game does not mark it, and it never suggests a rank you have not learned.
- **Action bars:** The Cooldown Manager's Key text shows the key on every icon, only for spells on buttons you can't see, or not at all. The default is only hidden buttons: a bar you turned off or shortened, or one shown only on mouse over or out of combat.
- **Action bars:** Every spell of every class and role now has one fixed button in the key layout. The spells you press in a fight are on the easy keys of your first two bars, and bar 3 holds what you use between pulls, such as buffs, resurrection and travel spells.
- **Action bars:** When a bar pages on Shift or Ctrl, or your text style hides the keys on bars 1 to 3, EldoUI tells you after you apply a key set and fixes it in one click.
- **Setup and layouts:** The Classic and Vanilla packs start the Keys and spells step on the Number row keys, the way the game sets bar 1.

### Fixed
- **Setup and layouts:** In the setup's UI scale step, a scale card with a long description no longer runs into the screen line above it or the custom scale below it, also with large text.
- **Setup and layouts:** In Edit Mode, the EldoUI side panel stays on screen when the list of what EldoUI places is open and long; the list scrolls instead.
- **Group frames:** In the Close Combat layout with the Healer role, the party frames no longer touch the top of your player frame.
- **Setup and layouts:** An interrupted first setup resumes unfinished changes, and a setup waiting for combat to end uses your latest layout choice.
- **Setup and layouts:** Finishing or skipping the first setup during combat now gives you your layout as soon as combat ends.
- **Setup and layouts:** EllesmereUI imports keep your chosen EldoUI layout's settings and responsive placement for frames the imported layout does not move.
- **Options:** Every line of a wrapped dialog checkbox label can be clicked without covering the buttons below it.
- **Notifications:** On a Hardcore character with the card title color set to Plain, as in the Quiet style, death and PvP cards show their title in plain white instead of the accent color.
- **Options:** Long page names in the options list and long page descriptions wrap onto a second line instead of being cut off, and a few choices with long names have shorter ones, in English and Danish.
- **General:** The update note's title, buttons and checkbox follow your selected language when you open it again.
- **General:** EldoUI keeps recognizing WoW: Forever if the game renames its client type at launch, so your characters' saved data and your look stay as they are.
- **Chat:** While you type in the main chat window with the input box over the tabs, a chat window you dragged out of the dock keeps its tab name, whisper icon and flash.
- **Unit frames:** 3D portraits stay inside the round portrait of the original frames and the portrait rings, with the face framed a little wider, and no dark square or box shows around the portrait or beside the target any more.
- **Unit frames:** The original frame art keeps its true shape on the Classic frames style, so its portrait ring sits exactly on the portrait, also on the target of target and the pet.
- **Unit frames:** Names stay inside their name bar or health bar in every unit frame style, and Classic frames show the level by the portrait instead of above the frame, where it could cover the target of target. A level badge on your own frame always shows your level.
- **Unit frames:** With the original frame art, the small circle under the player and target portraits shows the level, as on the classic frames: the rest icon while you rest, the attack icon in combat, and on the target a skull for a corpse or a level too high to tell.
- **Group frames:** The group pets and the main tanks no longer sit on top of each other next to a tall raid: the one you have turned on keeps the spot and the other goes beside it.
- **Saved settings:** EldoUI loads even when part of its saved settings file is damaged: a broken profile list or profile starts over as a new profile, and the damaged part is kept aside instead of being deleted.
- **Saved settings:** Import refuses a string that unpacks to more than the import size limit or carries damaged frame positions, with a clear message, before it changes any setting.
- **General:** /eui commands still work when you type a period, comma or other punctuation right after them, such as /eui errors.
- **Setup and layouts:** The durability figure moves aside with your buffs and debuffs when the minimap is larger or round, and on 16:10 screens, instead of sitting on top of them.
- **Paladin:** Training lists Righteous Fury at level 10 and Retribution Aura at its current trainer cost.
- **Shaman:** Training shows the current trainer costs and the level 50 rank for talented shamans, so the rank after it can show as well.
- **Performance:** The rare scanner reads the rare markers once for each burst of map updates instead of on every single update.
- **Action bars:** The keys of a bar that a layout hides keep working, also past a shortened bar's end. The hidden bar shows when you point at it out of combat, in a small box next to your bags (bars 4 to 8 at the right edge); a bar a layout switched off before comes back this way.
- **Setup and layouts:** A new character that starts on its class's profile keeps that profile when you run the full setup, instead of being moved to the shared EldoUI profile.
- **Journal:** Opening an attunement or a class quest from a link, a waypoint or a slash command scrolls the Attunements list to it, so its row is always in view.
