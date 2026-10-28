# Changelog

All notable changes to EldoUI, newest first. Each version starts with its highlights, then what is new, what was improved and what was fixed. Every line names the part of the UI it touches, and changes for one class carry the class name. Versions are listed as `[version] - date`.

The in-game **What's New** page (`/eui whatsnew`) shows the highlights of each version.

## [Unreleased]

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
- **Action bars:** A game shortcut a key set takes gets the same new key in every set, such as Alt-R for reply, and the game keys list (`/eui keys`) shows where bags, map and the rest are. Bar 3's last three keys use your potion, healthstone, and mana potion or bandage.
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

## [0.7.0002] - 2026-10-23

### Improved
- **General:** The install guide and the release notes name the WoW: Forever game folder, _forever_; the guide tells beta players to install EldoUI there again.
- **Journal:** The printable journal page uses the book fonts on your computer and no longer asks a web font site for its fonts when you open it.
- **Options:** The Version check option says that it sends your version as a hidden addon message to guild and group members who run EldoUI, never in chat.
- **General:** The note after an update has a "Never show again, even after updates" tick box; the switch on the What's new page turns the note back on.
- **Journal:** The copy box of a journal or runs backup code names the button to paste it into once, and the run count's tip says plainly that the Instances module records the runs.

### Fixed
- **General:** The bug report form and the support pages name the error window's Report button, as the game shows it.
- **Map and minimap:** Buttons on the minimap's side rail keep the rail's order, whichever one you put there first.
- **Group frames:** With the raid manager side panel skinned, the ready check, role poll, countdown and option buttons show their icons again.
- **Map and minimap:** With the Large minimap style, the Split Timer and the quest list move down with the bigger map instead of sitting under it, in every current layout.
- **Map and minimap:** On the world map, boat, zeppelin, Deeprun Tram and portal pins show a ship, an airship, a tram car and a swirl in their own colors, instead of plain colored blocks.
- **Action bars:** In Vanilla Original, the vehicle exit and zone ability buttons sit clear of the gryphons. The setup grays out the Large action bar style for this layout, since its bigger gryphons leave no room beside the bags.
- **Map and minimap:** With the minimap buttons skinned, the calendar button shows its calendar icon again.
- **Unit frames:** With the Classic frames style, the player and target portraits show the face at its true shape inside the Vanilla ring and the original portrait circle, and a new style or look updates the picture at once.
- **General:** After the micro menu's Mouse-over style, any other style shows the micro menu and the bag bar again, and the Mouse-over style's description says so.
- **Options:** Picking another style brings back the bars and buttons an earlier style hid or faded, such as the XP bar after Mouse-over only or the right chat panel after Split.
- **Windows and skins:** With the Modern (flat) look, every EldoUI window has an edge you can see against the world, and the options window steps aside while the setup is open and comes back after it.
- **Setup and layouts:** Vanilla Original's two right-edge columns and Modern Center's right-edge column hide their empty buttons, and Vanilla Original suggests Class Power pips without a second power bar, since its player frame already shows your power.
- **General:** The Info Bar's Two bars style keeps zone, coordinates, experience and reputation on its second bar, so nothing overlaps when that bar sits in the chat window.
- **Setup and layouts:** In move mode, the arrow keys nudge the selected frame, as its tip says: 1 unit, or 10 with Shift.
- **Journal:** The Loot Guide's PvP rewards list says why it is empty: the filters, with a button to clear them, or the loot data still loading, switched off or not installed. When the data arrives, every reward shows at once.
- **Localization:** In Danish, the Alts window's last-online column reads "Sidst set", the Journal's next trip reads "for level", and Reset size, the Macro Editor's subtitle and the Loot Guide's Dungeons caption are no longer cut off.
- **Journal:** The guild attunement list's "Seen" column is named "Sent", since it shows how long ago each member sent their data.
- **Localization:** With EldoUI in Danish, the options page subtitles, the Glows and Screen area tabs, the Safety page, the Blizzard UI switch notes, the search boxes, the Journal's place phrases and every date read Danish, with the day first.
- **Setup and layouts:** The Modern pack shows keybinds and macro names on the action buttons.
- **Setup and layouts:** In Modern Center, the cooldown Buff Bars sit clear of the pet and pet target frames.
- **Bags and loot:** The auction house tabs EldoUI adds are named Shopping List, Quick Sell and Cancel Undercut, so they no longer read like copies of Blizzard's Buy, Sell and Auctions tabs, and they stay inside the window with large text.
- **Setup and layouts:** Nameplate Focus turns the target of target frame off along with the target frame, so no lone frame is left on screen; another layout brings both back.
- **Unit frames:** On Boxed unit frames, the race and class text and the name keep clear of the class badge and the PvP and elite marks on the frame's corner.
- **Action bars:** Blizzard Bottom Block's two side grids hide their empty buttons, and show them while you drag a spell.
- **Journal:** The Loot Guide's dungeon list keeps the wing names of Dire Maul, Blackrock Spire, Scarlet Monastery and Stratholme, and the wishlist alert names the wing you entered.
- **Setup and layouts:** In EldoUI Center and Modern Center, the bag bar, the micro menu and the zone ability button stack in one column at the bottom right, clear of a damage meter docked in the corner.
- **Chat:** While you type in the chat box over the tabs, the tab names, whisper icons and new-message flashes no longer show through it.
- **General:** The Info Bar's memory block and its tooltip show the same total, and the open tooltip no longer adds work every few seconds.
- **Setup and layouts:** The setup's first click shows your layout's action bars right away, instead of a half-finished screen until you finish the setup.
- **Windows and skins:** The EldoUI button in the game menu is there from a new character's first login, before the setup is finished.
- **Setup and layouts:** EldoUI Center's second and third action bars hide their empty slots, so a new character's first screen no longer shows rows of empty boxes.
- **Journal:** Looting and moving items no longer makes the game hitch while the journal is open, and accepting or finishing quests no longer reworks the where-next list each time.
- **Unit frames:** An extra resource bar that shows its value as a percent no longer raises an error while the game keeps your power values hidden.

## [0.7.0001] - 2026-10-21

### Fixed
- **General:** Every EldoUI version can be downloaded as a zip from its release page.

## [0.7.0000] - 2026-10-21

### Highlights
- Ten built-in layouts with clearer names, and EldoUI Center as the new default for new profiles.
- Four roles in the setup and on the Role page: Melee, Ranged, Healer and Tank.
- A new Keys and spells step shows your keys, class spells and macros first and changes nothing on your bars until you press Apply.
- With the Vanilla Original skin, the unit frames, the action bar tray, the minimap border and the micro menu wear the game's own classic art.
- Every layout or pack change can be undone, from the alert after the change or with /eui layout undo.
- Your settings, layout, dragged frames and journal carry over to this version, and a copy is kept first that the new Saved data page can put back.
- EldoUI's own texts are now available in Danish, under General > EldoUI language.
- Nameplates, bags, cooldown displays and many other parts do much less work, and background work pauses in combat.

### New
- **Setup and layouts:** Ten built-in layouts, each with its own shape on screen: Vanilla Original, EldoUI Center, Modern Center, Blizzard Bottom Block, Portrait Staggered, Compact HUD, Widescreen Edges, Close Combat, Open Center and Nameplate Focus.
- **Setup and layouts:** EldoUI Center is the new default for new profiles: player and target sit level with the cooldown row, and the action bars form one block at the bottom with a narrow wing on each side. Profiles from earlier versions keep the layout they used.
- **Setup and layouts:** Four roles in the setup and on the Role page: Melee, Ranged, Healer and Tank. Ranged also shows the five-second rule on your mana bar.
- **Setup and layouts:** Every layout or pack change can be undone: press Undo on the alert after the change, or type /eui layout undo. Settings you changed yourself since stay as you set them.
- **Setup and layouts:** A new Keys and spells step, also on Express, shows your key preset, class spells, macros and rank upgrades before anything changes. Your bars change only when you press Apply, your own actions, macros, items and kept ranks stay, and one Undo puts it all back.
- **Setup and layouts:** In move mode, the pet and stance bars can be laid out Horizontal, Vertical or as a Grid, and the action bars, pet and stance bars, micro menu and bag bar have Size and Spacing menus.
- **Setup and layouts:** Move mode's frames menu has Find a frame: pick any frame to show, select and flash its box, and bring a frame that ended up off the screen back to the nearest edge.
- **Unit frames:** A new Classic frames style gives the player, target, target of target and pet frames the shape of the original frames, with a round portrait.
- **Unit frames:** With the Vanilla Original skin, frames sized like the originals wear the game's own classic frame art, with the elite and rare dragons on the target. The Vanilla Original layout shows them as soon as you pick it.
- **Action bars:** With the Vanilla Original skin, a one-row bar 1 sits on the classic stone tray with a gryphon at each end, the stance bar gets its classic stone, and the micro menu and bag slots wear their classic buttons.
- **Journal:** My Adventure keeps every dungeon and raid run with who was in it (name, class, level and role) and its loot rolls: who won which item and everyone's roll. Battlegrounds and arenas record nothing.
- **Journal:** Delete one run or one name from My Adventure with Undo. EldoUI never drops runs or companions on its own, and companion pages show what each companion won while grouped with you.
- **Map and minimap:** The Vanilla Original skin puts the game's own classic border around a round minimap, scaled with the map.
- **Saved settings:** Every update first keeps a copy of your settings and journal. The new Saved data page (or /eui data) puts a copy back, lists what a restore replaced so one click undoes it, and keeps any saved value EldoUI could not read aside instead of deleting it.
- **Localization:** EldoUI's own texts are available in Danish: pick Dansk under General > EldoUI language and reload. Game words players say in English, such as quest, loot and raid, stay English.
- **Localization:** The setup's first step lets you pick EldoUI's language, with the same flags as General > EldoUI language, and offers the reload right away.
- **General:** Mage Travel, the Party Quests panel, the Split Timer and the waypoint arrow can be set to show only in combat, out of combat, on mouse over or in a group, like the other HUD pieces.
- **General:** /eui probe textures lists which original interface textures your game client ships, ready to copy into a bug report.
- **Mage:** Mage Travel has five style presets: Standard, Small, Large, Quiet and Out of combat.

### Improved
- **Setup and layouts:** Picking a layout gives the same result from the Layouts page, /eui layout, the Overview, a pack and the setup: the layout's skin, Blizzard windows and suggested styles, nameplates included.
- **Setup and layouts:** Frames you dragged stay where you put them when you change layouts, unless you tick "Put frames I dragged back in the layout's spots". Applying the layout and look you already use changes nothing.
- **Setup and layouts:** If you picked a skin yourself, choosing a layout asks once whether to use the layout's look; "Keep my look" is the default.
- **Setup and layouts:** Layouts that left the list stay as legacy layouts, so your screen does not change after the update. If you had moved frames, a copy of your screen is also saved under your own layouts.
- **Setup and layouts:** One layout picker on the Layouts page, the Overview and the move panel: the ten layouts first, then legacy layouts you still use, then your own. The Overview and move mode show your layout, role, skin and Blizzard windows.
- **Localization:** General > EldoUI language shows each language's flag. The Danish texts come in a folder of their own that loads only when you pick Dansk, so playing in English uses no extra memory for them.
- **Localization:** With Dansk picked, menus, lists and window titles that still showed English now show Danish too, and so do the What's New page and the update note.
- **Setup and layouts:** A profile that used the older Damage role moves to your class's Melee or Ranged role by itself, and every frame stays where it was.
- **Setup and layouts:** The setup waits while the game asks whether to skip the intro cinematic, and while Details! or Questie show their own first-start windows, and opens once you have answered.
- **Setup and layouts:** The Other addons step in the setup lists only the addons EldoUI has a profile ready for, for your layout or specialization.
- **Unit frames:** A unit frame graphics choice that does not fit your layout is grayed out, with the reason in its tooltip.
- **Unit frames:** The unit and party frame style with the boxed 3D portrait and name bar is now called Boxed.
- **Group frames:** Party and raid frames keep the empty part of the health bar dark and clearly apart from the frame art in every skin, and the Minimal party style shows a slim mana bar on healers.
- **Nameplates:** Nameplates do much less work in big groups and cities: each plate listens only to its own unit, cast bars and hover update only while there is something to show, and quest progress and NPC titles are read once per change.
- **Nameplates:** EldoUI's nameplates wear your skin's frame edge, the same thin edge as small unit frames, and follow your unit frame graphics choice. Target, focus and style rule border colors still come first.
- **Action bars:** The class setup puts each key spell on the button of its keybind category, now including Shield Wall, Hammer of Justice, Freezing Trap, Frost Nova and Ice Block.
- **Action bars:** Cooldown rows show the key of another rank of a spell when that rank is on your bars, and spell buttons on the Consumable Bar, mounts included, show their cooldown without a global cooldown swipe.
- **Talents and spells:** The Planner row on Blizzard's talent window stays inside the window on small screens, and the Talent Planner tells you when Improve for Spellbook and talents is off.
- **Tooltips:** On the Tooltip page, a row whose module or switch is off is grayed and says why.
- **Journal:** Long run lists open one page of 100 runs at a time, and a journal with years of runs opens as fast as a new one. Runs and the people you ran with take about half the saved space, with nothing lost.
- **Map and minimap:** Show unexplored areas works from your first login: the parts of every zone you have not explored yet show dimmed, even where none of your characters has been.
- **Windows and skins:** Turning a window skin or the Mail module off puts Blizzard's look back at once, without a reload: spellbook, professions, quest and gossip dialogs, mailbox, friends, guild, calendar, PvP, the game menu and addon option windows.
- **Windows and skins:** Option gear panels, the Recent changes list, the setup's questions and help, the dungeon map and the journal's quick note share the look of EldoUI's other windows, and Escape closes the front one first.
- **Windows and skins:** Text sizes, tooltip titles and tooltip text match the rest of the interface in every window.
- **Notifications:** Alerts, the zone toast, rare cards and the low-mana note on a ready check share one queue: they no longer pile up, a repeated alert shows once, and alerts that waited out a long fight drop away.
- **Options:** Turning a module off or switching profiles asks for a reload only when a module really needs one, naming only the Blizzard parts that do. Switching a module on and off during a fight switches it once, after the fight.
- **Performance:** Bags, the vendor, the auction house, loot rolls, the Encounter Timeline, the Farming bar, Enemy Spotter, gathering pins and map coordinates redraw only what changed, and their timers run only while something is on screen.
- **Performance:** Cooldown rows, tracking bars, the cooldown pulse, the cursor ring, the Consumable Bar and the global cooldown bar share one cooldown reader, so a burst of cooldown changes redraws them once.
- **Performance:** Countdown bars, the ping feed, buff reminders, weapon enchant timers, minimap note pins, the quest tracker, waypoints, the Split Timer, Quickdraw and ActionCam work only while they show or are in use. Background work pauses in combat.
- **Performance:** The Loot Guide and waypoint arrows work out map positions with much less memory churn, Loot Guide search and the PvP page open faster, and the Loot Guide's side list waits until you open the window.
- **Performance:** Backups of a long journal and of years of runs are written a little at a time, so logging in after an update stays smooth.
- **Saved settings:** EldoUI records which version saved your settings. After an update every profile is brought forward without removing anything, settings you never changed keep the value you saw, and one chat line tells you.
- **Localization:** A name font you pick no longer replaces the font of Cyrillic, Korean or Chinese names, and name fonts stay in place when you change the theme font.
- **Localization:** The newest Loot Guide texts, such as run backups and loot rolls, are translated into German, French, Spanish, Portuguese, Russian, Korean and both kinds of Chinese.
- **General:** Changes EldoUI makes to Questie, RestedXP or Guidelime settings ask first, name the profile and the characters that share it, and can be undone. RestedXP's new guide window is placed on the layout's guide spot with its step list.
- **Shaman:** Totem timers kept with the totem bar move under or beside it when the cooldown rows fill the space above it, and tick only while a totem is out or an imbue runs.

### Fixed
- **Setup and layouts:** A profile that names a layout that is not installed now says so once and keeps your saved layout choice.
- **Setup and layouts:** A pack applied from the Overview or a pack string now also sets its role, and choosing the Healer pack after another pack no longer leaves raid frames covering your own frame.
- **Setup and layouts:** A micro menu or bag bar you moved in an older version stays where you put it, and the bar and macro check boxes on the class setup page remember your choice.
- **Unit frames:** Cast bars no longer show an error when an enemy casts something whose details the game keeps hidden, and keep the EldoUI look.
- **Unit frames:** Turning Unit Frames off brings Blizzard's own unit frames back at once, without a reload, unless they were set to be replaced.
- **Group frames:** With the Healer role, raids that use the Mid or Large raid settings keep the larger healer frames too.
- **Nameplates:** Turning off EldoUI's plate size after changing Blizzard's nameplate scale gives back the size the game uses now.
- **Action bars:** The zone ability's options, its box in move mode and its Blizzard UI switch name only the zone ability, and keybind mode no longer offers a key for an extra action button, which WoW: Forever does not have.
- **Talents and spells:** The Talent Planner, the Training tab and the spellbook skin go on and off together, whatever order you turn them on in.
- **Talents and spells:** With the game's gamepad interface on, EldoUI's buttons on the talent window, the spellbook and the trainer window step aside, and they come back when you switch to mouse and keyboard.
- **Tooltips:** Hovering an aura on an enemy nameplate in combat no longer causes an error with the smart tooltip position.
- **Journal:** Forgetting a character in the Alts window backs up its journal first and says so, and the newest backup of your runs from before an update is no longer pushed out by later restores or imports.
- **Journal:** The Attunements tab no longer lists WoW: Forever dungeons without a quest chain as empty pages; such a dungeon shows up once you have taken one of its quests.
- **Journal:** On a German client, quest objectives in the Loot Guide show in German.
- **Map and minimap:** Corner buttons on a small minimap no longer overlap.
- **Windows and skins:** Switching profiles or themes shows the new colors and skin right away, without a reload.
- **Options:** While the quest tracker is hidden by its Hide switch or its box, its visibility settings are grayed out and say why.
- **General:** Game windows, tooltips, nameplates, chat bubbles, the Training window and the Cooldown Manager no longer cause an error when the game hides a frame's layer or state from addons.
- **General:** Frames that fade out no longer cause an error when the game hides one of their parts from addons.
- **General:** Camp Helper recognizes every camp feature, the Anarchist's Workbench, Cookie's Feast and Iron Oven in any game language the first time you see them.
- **General:** The Durability info text shows its repair icon again.
- **General:** The camera no longer swings back and forth when you close one NPC window and open the next.
- **Paladin:** The blessing reminder, the Blessing Plan and the ready check report count only the blessings that share the blessing slot on WoW: Forever, so Salvation no longer counts as one, and Blessing of Sanctuary and Sanctity Aura are gone.
- **Shaman:** Water Shield and Rage of the Farseer work on the cooldown bar, the shield reminder and the class setup, Fire Nova has a ready icon, and Windfury and Flametongue Totem show on the party squares.
- **Shaman:** The totems and Earth Shield that WoW: Forever removed are gone from the pickers, and a saved pick of one goes back to the first one you know.

## [0.6.6005] - 2026-10-18

The versions from 0.5.0 to 0.6.6005 in short: what they brought that is still in EldoUI.

- **Setup and layouts:** A step-by-step setup with Express, a class setup for every class, a last page with "Revert this" for each change, and a once-per-login reminder for an unfinished setup.
- **Setup and layouts:** Preset packs (Modern, Classic, Vanilla, Healer and Minimal), UI amount (Essential, Moderate or Full), the Overview page with complete looks, and look strings to share.
- **Setup and layouts:** Move any frame with /eui move, hide a box with a right-click (a "Lock right-click" switch and a Hidden boxes page bring it back), and set keys with /eui kb.
- **Setup and layouts:** Imports of EllesmereUI, ElvUI and Edit Mode strings, and an ultrawide safe area.
- **Unit frames:** Unit frames with Blizzard element switches, heal prediction, text tags and cast bar effects, unit-frame graphics (Vanilla rings, Portrait Bars or the flat look), and a class resource bar with the five-second rule.
- **Group frames:** Party and raid frames with main tanks, group pets, raid sizes and click casting.
- **Action bars:** Eight action bars plus pet and stance bars, with fade and visibility rules, Fill order, proc glow and Masque, and keybind presets with a preview before any key changes.
- **Talents and spells:** The Talent Planner with Import build, pick order and a level-up checklist, Training with what your trainer teaches now and soon, and lower spell ranks lit on your bars, with Check ranks on the spellbook and /eui rankcheck.
- **Chat:** Saved history, search, keyword alerts, a spam filter, per-channel colors, and guild roster lines folded into one.
- **Tooltips:** Spell tooltips can show damage or healing per second and per mana, and the target or focus cast bar shows the spell's tooltip.
- **Bags and loot:** Bags and bank with your other characters' items and sections you can fold, merchant restock lists, the Loot Guide with best-in-slot sets and a wishlist, Raid Loot, Appearances and Farming history.
- **Journal:** My Adventure, a journal of your road from 1 to 60 told as a story, with backups and exports, and Attunements with raid keys, dungeon chains and class quests.
- **Map and minimap:** Dungeon Routes, Map Notes with the rares you met, Transport Maps, addon minimap buttons gathered behind one button, and a slim button rail.
- **Windows and skins:** Eight skins for the whole UI (Minimal Modern, Vanilla Original, Vanilla Refined, Warcraft Parchment, Forged Metal, Portrait Classic, Faction Heritage and Arcane), the Appearance page, panel tint, and skins for Blizzard's own windows.
- **Notifications:** Alert toasts with your choice of sound, the level-up card, the Ready Check Report and class reminders.
- **Options:** The Blizzard UI page with one switch per part of Blizzard's UI, the Visibility page with HUD presets, Recent changes with Undo, profiles that follow your character, talent group or content, and Large text, a High contrast skin, color-blind safe colors and sound cues.
- **Localization:** The Loot Guide in German, French, Spanish, Brazilian Portuguese, Russian, Korean and Chinese, and player names in Cyrillic, Korean and Chinese show their letters.
- **General:** The Info Bar with datatexts and a Dashboard, the error log (/eui errors) with a Report button that leaves out your character's name, realm, guild and chat text, Rare Scanner, the Encounter Timeline, Raid Tools with /eui pull, Combat Text and the Cooldown Manager.
- **General:** The Profession Planner, Finder, Macro Editor, Fishing, Streamer Mode, the Split Timer and Hardcore death alerts.
- **Mage:** Mage Travel lists the teleports and portals you know, and a mana gem button joins the Consumable Bar.
- **Paladin:** The Blessing Plan (/eui blessings) plans which blessing each paladin keeps up on each class.
- **Shaman:** Shaman Totems: a totem bar, a cooldown bar with your shield, weapon imbues, Reincarnation and Ankhs, up to eight totem loadouts, and a group plan for Mana Tide Totem and the resistance totems.

[Unreleased]: https://github.com/Eldodeldo/EldoUI/compare/v0.7.0002...HEAD
[0.7.0002]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0002
[0.7.0001]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0001
[0.7.0000]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.7.0000
[0.6.6005]: https://github.com/Eldodeldo/EldoUI/releases/tag/v0.6.6005
