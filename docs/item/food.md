# Custom Food

Type ID: `item:food`

### Fields:

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`max_count` | [Integer](../data_types/integer.md) | `64` | The maximum stack count for the item.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.
`hunger` | [Integer](../data_types/integer.md) | `4` | how many hunger it fills up (1 = half a bar).
`saturation` | [Float](../data_types/float.md) | `8.0` | How many saturation points the food fills.
`meat` | [Boolean](../data_types/boolean.md) | `false` | If set to true, you'll be able to use this item to feed dogs, and it will be identified as meat by the [Meat (Item Condition Type)](https://origins.readthedocs.io/en/latest/types/item_condition_types/meat).
`always_edible` | [Boolean](../data_types/boolean.md) | `false` | If set to true, this item will always be edible, even with full hunger.
`drinkable` | [Boolean](../data_types/boolean.md) | `false` | If true, makes you drink it as if it was milk or a potion.
`sound` | [Identifier](../data_types/identifier.md) | `"entity.generic.eat"` | The sound that plays while you are eating the item.
`returns` | [Identifier](../data_types/identifier.md) | *optional* | The item that this item returns when used.
`eating_time` | [Integer](../data_types/integer.md) | `30` | The amount of time (in ticks) the item will take to eat.

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
