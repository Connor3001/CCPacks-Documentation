# Custom Disc

Type ID: `item:music_disc`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](../data_types/string.md) | *optional* | Sets the items name.
`lore` | [Array](../data_types/array.md) of [String](../data_types/string.md) | *optional* | Lines of text below an item.
`item_powers` | [Array](../data_types/array.md) of [Item Power](../data_types/item_power.md) | *optional* | The powers your item will have.
`item_group`| [Item Group](../data_types/item_groups.md) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`comparator_output` | [Integer](../data_types/integer.md) | 1 | The signal strength a comparator outputs from this disc
`sound` | [Identifier](../data_types/identifier.md) | *mandatory* | the sound event that the disc uses.

### Example Code

```json
{
  "type": "item:music_disc",
  "comparator_output": 8,
  "sound": "example_pack:funky_sound"
}
```
