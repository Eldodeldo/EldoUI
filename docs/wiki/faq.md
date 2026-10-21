# FAQ

## Is EldoUI really made with AI?

Yes. EldoUI is designed and written with AI assistance, and every module is tested for WoW: Forever before it ships. It follows the same rules as any other addon: it only changes the interface and never plays for you.

## Does EldoUI work on Classic Era or Retail?

No. EldoUI is made for WoW: Forever (Interface 16001) and uses its API. It does not load on other game versions.

## Is EldoUI allowed under Blizzard's addon rules?

Yes. WoW: Forever limits what addons may do in combat, and EldoUI stays inside those limits: it changes how the UI looks and where things sit, and shows only what the game tells addons. It never plays for you (no automatic rolls, no automatic gear swaps) and never works out combat information the game hides. Where the game hides a value in combat, EldoUI shows the game's own display of it or nothing.

## The game says EldoUI is out of date

Tick **Load out of date AddOns** on the AddOns list of the character screen. This happens when Blizzard raises the interface number before a new EldoUI version is out.

## The Loot Guide says its data is not installed, or chat emoji do not show

The Loot Guide data (`EldoUI_LootData`), the gear simulator (`EldoUI_LootSim`), the emoji pictures (`EldoUI_Emoji`), and the Danish texts (`EldoUI_Locale_daDK`) are separate addon folders. They must sit directly in `Interface\AddOns`, next to `EldoUI`, not inside it. A release zip already has them in the right place.

## Another addon already does this. Do they clash?

No. EldoUI notices the addons you already use and steps back where they do the same job: Bags stays off while Bagnon, AdiBags or Baganator is loaded, Nameplates while Plater is loaded, and Action Bars while Bartender4 or Dominos is loaded. With addons that do many small things, such as Leatrix Plus, only the parts both do step back. You pick who handles each job on the Other addons page (`/eui addons`) or in the setup. See [Using EldoUI with other addons](other-addons.md).

## Where are my settings, and how do I start over?

Your settings live in `WTF\Account\<account>\SavedVariables\EldoUI.lua`. In game, `/eui profile reset` resets the profile you use, and `/eui install` runs the setup again. To keep your current setup safe first, `/eui export` gives you a share string you can import later.

## Can I use my setup on another character or share it?

Yes. Profiles can be shared by every character on the account (`/eui profile use <name>`), and `/eui export` makes a share string that someone else imports with `/eui import`. See [Layouts and presets](layouts.md#sharing-a-setup).

## Why do some changes ask for a reload?

A few settings only take effect after the UI reloads. Forever blocks addons from reloading on their own, so EldoUI shows a banner with a Reload button instead.

## A frame is in the wrong place

`/eui move`, then Shift-right-click the frame to put it back where the layout wants it. `/eui resetlayout` resets every frame.

## How do I report a problem?

1. Type `/eui errors` to open EldoUI's error log in its own window (the Errors tab in chat shows the same log).
2. Press **Report** on the error. It shows a ready-to-paste bug report with the version and setup details, and with your character's name, realm, guild and chat text left out.
3. Open the [bug form](https://github.com/Eldodeldo/EldoUI/issues/new?template=bug_report.yml), paste it in, and add a few words on what you were doing.

EldoUI never sends anything by itself: a report leaves the game only when you paste it.

For a problem without an error, `/eui diag copy` gives you the version and setup details as text. Screenshots help too.

## Who made EldoUI?

EldoUI is its own addon, written from scratch for WoW: Forever with AI assistance. The open-source code, data, fonts and sounds it builds on, and the work that inspired it, are credited in [Credits and third-party notices](../../THIRD_PARTY_NOTICES.md).

## I updated from 0.6 and my layout has a new name

Nine of the ten layouts got clearer names, and the ones that left the list stay as legacy layouts, so your screen does not change. [Updating from 0.6](updating-from-0-6.md) lists every old and new name.

## Can I play EldoUI in Danish?

Yes. Pick **Dansk** under General > **EldoUI language** in `/eui` and reload. EldoUI's own texts switch to Danish; the game's own texts keep the game's language.
