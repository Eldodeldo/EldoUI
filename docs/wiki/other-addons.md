# Using EldoUI with other addons

EldoUI recognizes supported addons and offers a choice for the jobs they share with EldoUI. It can step back for a whole module or for a supported individual feature. This is not a guarantee for every addon or combination; check who handles each job on the Other addons page.

## What steps back

- **A whole module.** Some addons own the same frames as an EldoUI module, so only one of them can run. Bags stays off while Bagnon, AdiBags or Baganator is loaded, Nameplates while Plater is loaded, and Action Bars while Bartender4 or Dominos is loaded.
- **Only the parts both do.** With addons that do many small things, EldoUI steps back only where they overlap. With Leatrix Plus, each shared feature (junk selling, repairs, faster loot, declining duels and invites, and a few more) steps back only while Leatrix Plus has the same feature switched on; the rest of EldoUI's Quality of Life features keep running. With TradeSkillMaster, EldoUI's Open All and address book in the mail step back, and the mail look stays. With ElvUI, each EldoUI module steps back only while ElvUI's own part for it is on: turn off ElvUI's bags and EldoUI's Bags runs.
- **Bars that move the same buttons.** The Micro Menu and the experience and reputation bars step back while a bar addon (Bartender4, Dominos, ElvUI) places the same buttons or bars.

An addon that loads later (load on demand) is noticed when it loads. Out of combat, EldoUI steps back and offers a reload so the change is complete.

## Picking who handles each job

Type `/eui addons page` to open **Other addons** in the config window. Every addon EldoUI found is listed with each job it shares and who handles it now.

- **Use EldoUI's** gives the job to EldoUI. For a whole module, the other addon is turned off for this character after a reload. For a part both can run, EldoUI's part turns on right away and the other addon stays on.
- **Keep** *(addon name)* leaves the job to the other addon and EldoUI steps back again. If you turned that addon off with Use EldoUI's and haven't reloaded yet, Keep turns it back on.
- **Turn off** *(addon name)* shows for addons whose jobs all run next to EldoUI's. It turns the addon off for this character, after a reload.

Your picks are saved for your whole account, so they stay through reloads and profile switches. EldoUI never turns another addon on or off without your click.

In chat: `/eui addons` lists what was found, `/eui addons use <addon>` and `/eui addons keep <addon>` pick for one addon, and `/eui addons page` opens the page.

The first time EldoUI finds an addon it leaves a job to, it says so with one chat line. Turn that line off with **Chat line when an addon is found** on the Other addons page.

## In the setup

When EldoUI finds an addon on your first login, the setup has a step **Addons you already use**. Each job has two cards: **EldoUI** (marked Recommended) and **Keep** *(addon name)*. Nothing changes before Finish, and Finish names every addon it turns off. Express setup takes the recommended pick. On the last page, **Revert this** turns those addons back on.

## Addons in your layout

Your layout also has spots for the frames of supported addons you keep. Out of combat, EldoUI places and sizes their frames on the layout's spot for that job and moves them along when you pick another layout. EldoUI's own frame for the same job steps aside while the other addon has the spot.

- Supported: XLoot (loot window, roll bars and loot feed), SilverDragon and RareScanner (on the rare card), Bagnon, BetterBags and Baganator (bag and bank corners), MinimapButtonButton (the minimap's button bin corner), TellMeWhen (the first six icon groups on the aura icon spots), TomTom (the waypoint arrow spot), Titan Panel (the data bar edge), HealBot Continued (the party spot, and the raid spot in a raid), and WeaponSwingTimer and 4everSwingTimer (the swing timer spots).
- **Layout spots for other addons** on the Other addons page lists each one with its state. Turn off **Place other addons in the layout** to leave all of them where their own settings put them, or **Place** *(addon name)* to do that for one.
- Where an addon keeps a spot of its own, **Save the spot in** *(addon name)* writes the layout's spot into that addon's own settings, so it stays there without EldoUI too. You see every value first, and **Undo** puts them back.
- In chat: `/eui addons fit` lists them, and `/eui addons fit on` or `off`, with or without an addon name, switches the spots.

## Addons that work alongside EldoUI

Some addons are made to work with EldoUI and never make it step back: EldoUI places Details!, BigWigs, Deadly Boss Mods and others in your layout and sets them up from the setup's Other addons step (`/eui install addons`).

## For addon authors

Plugins declare which addons do the same job as their modules in the same way. See [Other addons that do the same job](../PLUGINS.md#other-addons-that-do-the-same-job) in the plugin guide.
