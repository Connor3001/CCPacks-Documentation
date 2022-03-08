# Custom Food

### Fields:

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`item_powers` | [Item Power [array]]() | *optional* | The powers your item will have.
`max_count` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *64* | The maximum stack count for the item.
`hunger` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *4* | how many hunger it fills up (1 = half a bar)
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`saturation` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *8f* | How many saturation points the food fills
`meat` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *false* | Can it be fed to dogs?
`always_edible` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *false* | Can you eat it even when full?
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.
`drinkable` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *false* | If true, makes you drink it as apposed to eating.
`sound` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *false* | The sound you play while you are eating it
`returns` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *false* | The item that this item returns when used.
`eating_time` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *false* | The amount of time (in ticks) it takes to eat

### Example Code:

```json
{
    "type": "item:food",
    "max_count": 64,
    "hunger": 8,
    "saturation": 12,
    "meat": false,
    "always_edible": true,
    "returns": "minecraft:diamond",
    "drinkable": false,
    "sound": "minecraft:block.sand.place",
    "eating_time": 60
}
```
