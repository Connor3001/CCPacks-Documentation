# Custom Tools

Type IDs: `item:axe`, `item:pickaxe`, `item:shovel`, `item:hoe`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | `100` | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `"misc"` | The tab you can find the item in.
`start_colour` | [Colour](../data_types/colour.md) | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Colour](../data_types/colour.md) | *optional* | The end colour gradient of the Durability bar.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.
`mining_speed_multiplier` | [Float](../data_types/float.md) | `0.0` | (unknown, if you know, tell me on the discord)
`attack_damage` | [Integer](../data_types/integer.md) | `0` | the amount of damage that a weapon does.
`attack_speed` | [Integer](../data_types/integer.md) | `0` | How fast you can swing the weapon.
`mining_level` | [Integer](../data_types/integer.md) | `0` |
`enchantability` | [Integer](../data_types/integer.md) | `0` | How likely you are to get good enchantments.
`repair_item` | [Identifier](../data_types/identifier.md) | *optional* | The item used to repair this item.

### Example Code

```json
{
    "type": "item:axe",
    "durability": 450,
    "mining_speed_multiplier": 10,
    "attack_damage": 11,
    "attack_speed": 1.1,
    "mining_level": 4,
    "enchantability": 12,
    "lore": [
        "a fragile tool and weapon"
    ]
}
```
