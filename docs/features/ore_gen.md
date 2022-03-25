# Ore Generation

Type ID: `feature:ore_generation`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`block` | [Identifier](../data_types/identifier.md) | *mandatory* | The block that will be created by the generation.
`vein_size` | [Integer](../data_types/integer.md) | 9 | The amount of ore blocks to be made per vein.
`veins_per_chunk` | [Integer](../data_types/integer.md) | 20 | The amount of veins in one chunk.
`min_height` | [Integer](../data_types/integer.md) | 0 | The lowest Y value you can find the ore at.
`max_height` | [Integer](../data_types/integer.md) | 64 | The highest Y value you can find the ore at.

### Example Code

```json
{
    "type": "feature:ore_generation",
    "block": "example_pack:kunzite_ore_gravel",
	"vein_size": 9,
	"veins_per_chunk": 20,
	"min_height": 0,
	"max_height": 64
}
```
