# Custom Armor

Type ID: `item:armor`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | Sets the items name.
`lore` | [Array](../data_types/array.md) of [String](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Power](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | *10* | How many uses the item has.
`slot` | [String](../data_types/string.md) | *optional* | Which equipped item to execute the action on. One of: `"head"`, `"chest"`, `"legs"`, `"feet"`.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`texture` | [String](../data_types/string.md) | *mandatory* | The name of the image files used to texture the armor.
`protection` | [Integer](../data_types/integer.md) | *0* | the amount of damage that a weapon does.
`toughness` | [Integer](../data_types/integer.md) | *0* | the amount of damage that a weapon does.
`knockback_resistance` | [Integer](../data_types/integer.md) | *0* | How fast you can swing the weapon.
`enchantability` | [Integer](../data_types/integer.md) | *0* | How likely you are to get good enchantments.
`repair_item` | [Identifier](../data_types/identifier.md) | *optional* | The item used to repair this item.

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
