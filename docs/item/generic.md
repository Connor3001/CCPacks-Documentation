# Custom Items

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`max_count` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *64* | The maximum stack count for the item.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.

### Example Code

```json
{
	"type": "item:generic",
	"item_group": "materials",
	"max_count": 64
}
```
