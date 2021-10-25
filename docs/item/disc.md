# Custom Disc



### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`sound` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *mandatory* | the sound event that the disc uses.
`comparator_output` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | 1 | The signal strength a comparator outputs from this disc

### Example Code

```json
{
  "type": "item:music_disc",
  "comparator_output": 8,
  "sound": "example_pack:funky_sound"
}
```
