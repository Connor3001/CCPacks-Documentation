# Ore Generation

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`block` | [Block](../submodules/apoli-docs/docs/data_types/data_types/block.md) | *mandatory* | The block that will be created by the generation.
`vein_size` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | 9 | The amount of ore blocks to be made per vein.
`veins_per_chunk` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | 20 | The amount of veins in one chunk.
`min_height` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | 0 | The lowest Y value you can find the ore at.
`max_height` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | 64 | The highest Y value you can find the ore at.

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
