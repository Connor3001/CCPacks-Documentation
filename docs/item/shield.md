# Custom Shield

Type ID: `item:shield`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | Sets the items name.
`lore` | [Array](../data_types/array.md) of [String](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Power](../data_types/item_power.md) | *optional* | The powers your item will have.
`durability` | [Integer](../data_types/integer.md) | *100* | How many uses the item has.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`start_colour` | [Colour](../data_types/colour.md) | *optional* | The start colour gradient of the Durability bar.
`end_colour` | [Colour](../data_types/colour.md) | *optional* | The end colour gradient of the Durability bar.
`fuel_tick` | [Integer](../data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`cooldown` | [Integer](../data_types/integer.md) | *60* | How long the shield takes to be able to be used again when struck with an axe.
`enchantability` | [Integer](../data_types/integer.md) | *0* | How likely you are to get good enchantments.
`repair_item` | [Identifier](../data_types/identifier.md) | *optional* | The item used to repair this item.

### Example Code

```json
{
    "type": "item:shield",
    "cooldown": 20,
    "durability": 100,
    "enchantability": 9
}
```
