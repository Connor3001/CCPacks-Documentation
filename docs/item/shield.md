# Custom Shield

Type ID: `item:shield`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | The display name of the item. Can be a literal string or a translation key. If none is given, it'll default to `item.namespace.path`.
`lore` | [Array](../data_types/array.md) of [Strings](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Powers](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | `100` | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `"misc"` | The tab you can find the item in.
`start_colour` | [Colour](../data_types/colour.md) | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Colour](../data_types/colour.md) | *optional* | The end colour gradient of the Durability bar.
`fuel_tick` | [Integer](../data_types/integer.md) | `0` | How long the item can smelt for in a furnace.
`cooldown` | [Integer](../data_types/integer.md) | `60` | How long the shield takes to be able to be used again when struck with an axe, in ticks.
`enchantability` | [Integer](../data_types/integer.md) | `0` | How likely you are to get good enchantments.
`repair_item` | [Identifier](../data_types/identifier.md) | *optional* | The item used to repair this item.

[//]: # "TODO: Explain how the `enchantability` field works. Is it a percentage? Does it have a limit?"

### Example Code

```json
{
    "type": "item:shield",
    "cooldown": 20,
    "durability": 100,
    "enchantability": 9
}
```
