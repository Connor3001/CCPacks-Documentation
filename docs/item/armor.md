# Custom Armor

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`name` | [String](../submodules/apoli-docs/docs/data_types/string.md) | *mandatory* | The name of the image files used to texture the armor.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`slot` | [String](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Which equipped item to execute the action on. One of: `"head"`, `"chest"`, `"legs"`, `"feet"`.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *10* | How many uses the item has.
`protection` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | the amount of damage that a weapon does.
`toughness` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | the amount of damage that a weapon does.
`knockback_resistance` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How fast you can swing the weapon.
`enchantability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How likely you are to get good enchantments.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.
`repair_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The item used to repair this item.

### Armor json structure

```json
{
	"type": "item:armor",
	"slot": "chest",
	"name": "kunzite",
	"durability": 750,
	"protection": 5,
	"toughness": 1,
	"knockback_resistance": 0,
	"enchantability": 6,
	"item_group": "materials"
}
```
