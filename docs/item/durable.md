# Custom Durable Items

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`name` | [String](../../data_types/string) | *optional* | Sets the items name.
`repair_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The item used to repair this item.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *mandatory* | How many uses the item has.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`start_colour` | [Color Holder]() | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Color Holder]() | *optional* | The end colour gradient of the Durability bar.
`item_powers` | [Item Power [array]]() | *optional* | The powers your item will have.

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
