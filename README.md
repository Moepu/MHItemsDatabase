# moepu.boo

This wiki is powered by item data stored in [`data/items.json`](https://github.com/Moepu/MHItemsDatabase/blob/main/items.json). If you want to contribute, the main way to help is by submitting additions or fixes to that file.

## How To Contribute

Add a new item object or update an existing one in [`data/items.json`](https://github.com/Moepu/MHItemsDatabase/blob/main/items.json) using this structure:

```json
{
  "id": ID, // Number
  "name": "Item Name", // Text
  "description": "Description of The Item", // Rich Text
  "category": "Category of The Item", // Text
  "tier": "Tier", // Text
  "imageUrl": "https://static.wikia.nocookie.net/the-miners-haven-project/images/7/77/Airborne_Pathogenic_Spewer.png", // URL
  "wikiUrl": "https://minershaven.fandom.com/wiki/Airborne_Pathogenic_Spewer", // URL
  "properties": { // This is just an example, you can add custom Property as long as it is correct to the original or in-game.
    "Tier": "Enchanted",
    "Item Size": "9x12x15",
    "Date Added": "29 October, 2025",
    "Created By": "Jessssssssss_s|Supz_Boi",
    "Effects": "Base multiplier of x200 · Increased multiplier with certain status effect · Maximum upgrade of x3200",
    "Drawbacks": "''Plague'' increase ore size by 10% after 5 seconds if not cured · Plague kills ores after 15 times of size increase · '''Bypasses shields'''",
    "Source": "The Craftsman",
    "Requirements": "Scorponyte Mine x3 · Mycolympus x1 · Son of Poison x6 · Bubonic Plague x10 · Venomshank x5 · Sinister Sepulcher x1 · Ghosdeeri's Antidote x5 · 750 Shards",
    "Conveyor Speed": "200%",
    "Conveyor Wall": "Yes",
    "Conveyor Elevation": "Ground",
    "Upgrade Limit": "1 (Resettable)",
    "Upgrade Counter": "3",
    "Reborn Proof": "Yes",
    "Soulbound": "Yes",
    "Sell Value": "Can't Sell",
    "Cost": "''See Item Requirements''",
    "MPU": "x1.801 (base) · x2.451 (max)"
  }
}
```

Everything outside of `properties` should keep this same structure:

- `id`
- `name`
- `description`
- `category`
- `tier`
- `imageUrl`
- `wikiUrl`
- `properties`

The fields inside `properties` are flexible. Each entry is automatically shown as its own detail card in the wiki, so you can add missing info like `MPU`, a hint, special notes, mechanics, or any other useful detail. Besides the name of the item, every text field is considered RichText so that you can add color or format the text to however you like.

When you're done, you can submit your merge request and me or someone else will merge it if it's factual.
