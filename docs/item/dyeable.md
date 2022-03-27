# Custom Items

Type ID: `item:dyeable`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../../data_types/string) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`max_count` | [Integer](../data_types/integer.md) | `64` | The maximum stack count for the item (Max: 64).
`item_group`| [Item Group](../data_types/item_groups.md) | `"misc"` | The tab you can find the item in.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.

### Example Code

```json
{
	"type": "item:dyeable",
	"item_group": "materials",
	"max_count": 64
}
```
