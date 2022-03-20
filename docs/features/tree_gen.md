# Tree Generation

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`log_block` | [Block](../submodules/apoli-docs/docs/data_types/data_types/block.md) | *mandatory* | The block that will be the log of the tree.
`leaf_block` | [Block](../submodules/apoli-docs/docs/data_types/data_types/block.md) | *mandatory* | The block that will be the leaves of the tree.
`sapling_block` | [Block](../submodules/apoli-docs/docs/data_types/data_types/block.md) | *mandatory* | The block that will be the sapling of the tree.
`log_height` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | 4 | The amount of logs tall that the tree is.
`log_variance` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | 2 | How many blocks the tree height can vary by.
`leaf_radius` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | 2 | The radius of the leaves on the tree.
`leaf_offset` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | 0 | The height offset for where the leaves are made.
`leaf_height` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | 3 | The amount of leaves tall the tree is.
`chance_per_chunk` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | 33 | the % chance of a tree appearing per chunk (0-100).

### Example Code

```json
{
    "type": "feature:tree",
    "log_block": "minecraft:quartz_pillar",
    "leaf_block": "minecraft:oak_leaves",
    "sapling_block": "minecraft:grass"
}
```
