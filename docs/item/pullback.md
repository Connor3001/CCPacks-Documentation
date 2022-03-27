# Custom Items

Type ID: `item:pullback`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../../data_types/string) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | `1` | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`start_color` | [Colour](../data_types/colour.md) | *optional* | The start colour gradient of the Durability bar.
`end_color` | [Colour](../data_types/colour.md) | *optional* | The end colour gradient of the Durability bar.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.
`entity_type` | [Identifier](../data_types/identifier.md) | *optional* | The entity fired when you finish pulling it back.
`max_speed` | [Float](../data_types/float.md) | `3.0` | The maximum speed it will launch a projectile at.

[//]: # "TODO: explain how the `max_speed` float works. How do you calculate the amount of time it takes to pullback the item depending on the speed?"

### Example Code

```json
{
	"type": "item:pullback",
	"item_group": "none"
}
```
