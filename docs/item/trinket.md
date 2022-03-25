# Custom Trinkets

There is a [wiki for Trinkets](https://github.com/emilyalexandra/trinkets/wiki) that will help with getting trinkets set up.

Type ID: `item:trinket`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../../data_types/string) | *optional* | Sets the items name.
`lore` | [Array](../data_types/array.md) of [String](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Power](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | *optional* | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`start_color` | [Colour](../data_types/colour.md) | *optional* | How many uses the item has.
`end_color` | [Colour](../data_types/colour.md) | *optional* | How many uses the item has.
`fuel_tick` | [Integer](../data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.

### Example Code

```json
{
	"type": "item:trinket"
}
```
