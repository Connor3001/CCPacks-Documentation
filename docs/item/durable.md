# Custom Durable Items

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`durability` | [Integer]() | *mandatory* | How many uses the item has.
`lore` | [String [array]]() | *optional* | Lines of text below an item.

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
