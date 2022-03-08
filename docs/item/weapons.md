# Custom Weapons

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`item_powers` | [Item Power [array]]() | *optional* | The powers your item will have.
`start_colour` | [Color Holder]() | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Color Holder]() | *optional* | The end colour gradient of the Durability bar.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *10* | How many uses the item has.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`attack_speed` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How fast you can swing the weapon.
`attack_damage` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | the amount of damage that a weapon does.
`enchantability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How likely you are to get good enchantments.
`repair_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The item used to repair this item.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.

### Example Code

```json
{
    "type": "item:sword",
    "durability": 550,
    "mining_speed_multiplier": 0,
    "attack_damage": 8,
    "attack_speed": 1.7,
    "mining_level": 0,
    "enchantability": 12,
    "lore": [
        "a fragile weapon"
    ]
}
```
