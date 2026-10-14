# FAQ

## Is EldoUI really made with AI?

Yes. EldoUI is designed and written with AI assistance, and every module is tested for WoW: Forever before it ships. It follows the same rules as any other addon: it only changes the interface and never plays for you.

## Does EldoUI work on Classic Era or Retail?

No. EldoUI is made for WoW: Forever (Interface 16001) and uses its API. It does not load on other game versions.

## Is EldoUI allowed under Blizzard's addon rules?

Yes. WoW: Forever applies the Midnight addon restrictions, and EldoUI stays inside them: it changes how the UI looks and where things sit, and shows only what the game tells addons. It never plays for you (no automatic rolls, no automatic gear swaps) and never works out combat information the game hides. Where the game hides a value in combat, EldoUI shows the game's own display of it or nothing.

## The game says EldoUI is out of date

Tick **Load out of date AddOns** on the AddOns list of the character screen. This happens when Blizzard raises the interface number before a new EldoUI version is out.

## The Loot Guide says its data is not installed, or chat emoji do not show

The Loot Guide data (`EldoUI_LootData`), the gear simulator (`EldoUI_LootSim`), and the emoji pictures (`EldoUI_Emoji`) are separate addon folders. They must sit directly in `Interface\AddOns`, next to `EldoUI`, not inside it. A release zip already has them in the right place.

## Another addon already does this. Do they clash?

A module stays off while an addon that does the same job is loaded: for example Bags while Bagnon, AdiBags or Baganator is loaded, Nameplates while Plater is loaded, or Action Bars while Bartender4 or Dominos is loaded. Turn the other addon off if you want EldoUI's version.

## Where are my settings, and how do I start over?

Your settings live in `WTF\Account\<account>\SavedVariables\EldoUI.lua`. In game, `/eui profile reset` resets the profile you use, and `/eui install` runs the setup again. To keep your current setup safe first, `/eui export` gives you a share string you can import later.

## Can I use my setup on another character or share it?

Yes. Profiles can be shared by every character on the account (`/eui profile use <name>`), and `/eui export` makes a share string that someone else imports with `/eui import`. See [Layouts and presets](layouts.md#sharing-a-setup).

## Why do some changes ask for a reload?

A few settings only take effect after the UI reloads. Forever blocks addons from reloading on their own, so EldoUI shows a banner with a Reload button instead.

## A frame is in the wrong place

`/eui move`, then Shift + right-click the frame to put it back where the layout wants it. `/eui resetlayout` resets every frame.

## How do I report a problem?

1. Type `/eui errors` to open EldoUI's error log in its own window (the Errors tab in chat shows the same log).
2. Select the error and use the issue button: it copies the error with the version and setup details, ready for a GitHub issue.
3. Open a new issue on the [issue tracker](https://github.com/Eldodeldo/EldoUI/issues), paste it in, and add a few words on what you were doing.

For a problem without an error, `/eui diag copy` gives you the version and setup details as text. Screenshots help too.

## Who made the layouts and features?

EldoUI is its own addon. A few parts adapt open-source code under their own licenses (What's Training?, Molinari, and Forever Journal), fifteen layouts take their general idea from public community presets, and many features were inspired by well-loved addons. Everyone is credited in [Credits and third-party notices](../../THIRD_PARTY_NOTICES.md).
