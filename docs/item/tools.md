# Custom Tools

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *10* | How many uses the item has.
`mining_speed_multiplier` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *0* | (unknown, if you know, tell me on the discord)
`attack_damage` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | the amount of damage that a weapon does.
`attack_speed` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How fast you can swing the weapon.
`mining_level` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | doesn't actually do anything on swords.
`enchantability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How likely you are to get good enchantments.
`repair_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The item used to repair this item.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.

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
