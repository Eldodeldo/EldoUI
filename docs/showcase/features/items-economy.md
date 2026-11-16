# Items & Economy

Your bags, your gold and the items you are after.

[Back to the overview](../overview.md)

## Bags

All bags and the bank in EldoUI windows with categories and a bag bar, item counts across your characters in the tooltip, search with filters, offline viewing and a Blizzard skin mode. Items you already know are tinted, and sorting happens only when you click. `/eui find <text>` searches the items of all your characters; `/eui bank` shows your saved bank anywhere.

Junk coins and dimmed icons in live bags follow Merchant's sell and keep rules while that module is on, including its quest, recipe, equipment-set, and refund protection. The same marks appear in the game's bag windows when their extra information is enabled. With Merchant off, gray items receive the marks.

Ctrl+Alt+right-click an item in EldoUI's bags or bank to change its junk rule. A gray item switches Never sell, and other items switch Always sell. The modifier pair can be changed or disabled in Merchant settings. The coin, Junk category and tooltip update together.

The footer shows free general slots and warns as space runs low. Choose Used of total for the previous count format. Hover the count for each bag's capacity, or the count and gold for vendor values and saved usual auction prices grouped by item kind. Nearly full bags can mark their lowest-value eligible stack. The Loot window names the same stack after the game reports that an item does not fit. Both cues have their own switches.

## Bag Actions

Alt-click an item in your bags to disenchant it, or Alt-click a lockbox to pick its lock, when you know the profession. You choose the modifier, keep items safe with an exclude list, and set the highest quality it will disenchant. Rows for professions Forever doesn't have stay hidden. The module is off until you turn it on, and nothing happens without your click.

## Loot Guide

A loot journal for dungeons and raids, best-in-slot sets, a wishlist, search and item pages, and loot lines in item tooltips. The data (drops, chances, creatures and quests) comes from the separate EldoUI_LootData folder, which is generated from CMaNGOS classic-db: Classic values, so WoW: Forever may differ. Open it with `/lg`. All nine WoW: Forever dungeons have their own pages with their level range and zone; a boss joins its page the first time you defeat it, with the items you see it drop.

## My Adventure

Your character's journal, as the first tab of the Journal window (`/eui journey`). It writes itself as you play: levels, places, dungeons and bosses, quests with who gave them, finds, the people you traveled with, and your own goals and notes with reminders. It tells it back as a Journey by level, day, or zone, as a Book from level 1 to 60 in the tone you pick, as keepsake cards, and as a character card for your screenshot. Every dungeon and raid run is kept with who was in it and its loot rolls: who won which item and everyone's roll. Next trips suggests dungeons, quests, and attunement steps that fit your level. Moments show in the alert lane and a small tracker sits under your quests. It writes down only what the game shows you and never acts for you. Moving from Forever Journal keeps your history. More on [its wiki page](../../wiki/my-adventure.md).

## Upgrades

Upgrade arrows from a stat-weight scale in tooltips, bags, merchants, loot rolls and quest rewards. Gems and enchants count, and Pawn scales can be imported and exported.

## Auction House

Shopping lists, quick selling with price checks, canceling, full scans, crafting costs, disenchant values and a price database for the auction house.

Shopping also shows deals from searches and full scans you start. Set a target price on the watch list, open an exact result in Buy, and see a warning when your proposed sale is far below the usual price.

Item tooltips show the last auction price and a usual price once your searches cover at least three days. An arrow marks three days of clearly higher or lower prices, and the tooltip says when a vendor pays more after the auction house takes its share. Hold Shift for the last seven daily lows. Quick Sell suggests the usual price if there are no current listings and you have no remembered price.

## Merchant

Repair (from guild funds first, then your own) and sell gray items when you open a merchant, both with a switch, restock to exact amounts, fill ammo, and an item list for the merchant window. `/eui restock` opens the restock list.

Keep every sale undoable limits automatic junk selling to one batch of up to 12 stacks per visit, with the number left shown in the sale summary. It is off by default. When it is off, selling continues in batches, and the buyback tab holds the last 12 sold stacks.

The Sell junk button shows the eligible stack count and value when Merchant Improve is enabled. Each click sells at most twelve stacks and works with automatic selling on or off.

## Mail

Open all, select several letters and return them, an address book and a log of the mail you sent (`/eui sentmail`).

## Trade

The trade window in the EldoUI look on its own mover, who you trade with, what each side's items are worth, and a log of gold trades (`/eui trades`).

## Mob and Loot Info

Tracks what you loot from each mob and shows drop rates in item and mob tooltips.

## Alts

An Alts window with every character you log in on: an overview table with level, rested XP, gold and played time, plus tabs for search across all bags, banks, mail and auctions, professions and recipes, mail and auctions, quests, grids for gear, reputation, currencies and lockouts, a character page, a level log and an agenda with reminders. Recipe tooltips and vendors show which of your characters know or can learn a recipe. Each character records itself at login; nothing is ever sent unless you turn on the guild exchange and click. Steps back while Altoholic or DataStore is loaded. `/eui alts` opens the window.

## Appearances

A small mark on item buttons in your bags and bank, at vendors, in loot windows and rolls, and in the mailbox tells you whether you already have the item's look, have it from another item, or can't collect it. The item tooltip gets an "Appearance:" line, and the Loot Guide's Sets page counts the looks you have per set. Pick an icon, a colored corner or a text badge.

## Profession Planner

Pin recipes with a number of crafts, from the profession window, the Loot Guide's Crafting page or the Alts window. The planner lists every reagent, sub-reagents included, with what you have in bags, bank and on your other characters, recipe cooldowns and missing prices. A tracker shows what is left to buy, "Send to Shopping" fills an auction house shopping list, and a leveling plan picks the cheapest recipes up to the skill you want. `/eui plan`.

## Zone Quests

The Loot Guide Catalog gets a Zones section (`/eui zones`) that lists every zone's done and remaining quests with their givers and chains, with filters. Quest giver pins on the world map are optional (off by default, five pin looks), and the zone tooltip gets a "Quests done / total" line.

## Quest Starter Drops

Creature tooltips get a "quest starter" line, and EldoUI nameplates a small icon, when the creature can drop an item that starts a quest. The hint hides when the quest is done, taken or not for you, or when the item is already in your bags, and a minimum drop chance keeps rare drops out.
