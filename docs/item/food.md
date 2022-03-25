# Custom Food

Type ID: `item:food`

### Fields:

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | Sets the items name.
`lore` | [Array](../data_types/array.md) of [String](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Power](../data_types/item_power.md) | *optional* | The powers your item will have.
`max_count` | [Integer](../data_types/integer.md) | *64* | The maximum stack count for the item.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`hunger` | [Integer](../data_types/integer.md) | *4* | how many hunger it fills up (1 = half a bar)
`saturation` | [Float](../data_types/float.md) | *8f* | How many saturation points the food fills
`meat` | [Boolean](../data_types/boolean.md) | *false* | Can it be fed to dogs?
`always_edible` | [Boolean](../data_types/boolean.md) | *false* | Can you eat it even when full?
`drinkable` | [Boolean](../data_types/boolean.md) | *false* | If true, makes you drink it as apposed to eating.
`sound` | [Identifier](../data_types/identifier.md) | *false* | The sound you play while you are eating it
`returns` | [Identifier](../data_types/identifier.md) | *false* | The item that this item returns when used.
`eating_time` | [Integer](../data_types/integer.md) | *false* | The amount of time (in ticks) it takes to eat

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
