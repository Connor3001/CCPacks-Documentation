# Custom Durable Items

Type ID: `item:durable`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../../data_types/string) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | `100` | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `"misc"` | The tab you can find the item in.
`start_colour` | [Colour](../data_types/colour.md) | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Colour](../data_types/colour.md) | *optional* | The end colour gradient of the Durability bar.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.

### Example Code

```json
{
	"type": "item:durable",
	"item_group": "materials",
	"durability": 100,
	"max_count": 64,
	"start_color": {
		"red": 0.85882352941,
		"green": 0.45882352941,
		"blue": 0.92156862745
	},
	"end_color": {
		"red": 0.62352941176,
		"green": 0.07843137254,
		"blue": 0.70980392156
	}
}
```
