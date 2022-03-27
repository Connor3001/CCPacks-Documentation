# Tree Generation

Type ID: `feature:tree`

### Fields

  Field              | Type                                    | Default | Description
-------------------|-------------------------------------------|---------|-------------
`log_block`        | [Identifier](../data_types/identifier.md) |         | The block that will be the log of the tree.
`leaf_block`       | [Identifier](../data_types/identifier.md) |         | The block that will be the leaves of the tree.
`sapling_block`    | [Identifier](../data_types/identifier.md) |         | The block that will be the sapling of the tree.
`log_height`       | [Integer](../data_types/integer.md)       | `4`     | The amount of logs tall that the tree is.
`log_variance`     | [Integer](../data_types/integer.md)       | `2`     | How many blocks the tree height can vary by.
`leaf_radius`      | [Integer](../data_types/integer.md)       | `2`     | The radius of the leaves on the tree.
`leaf_offset`      | [Integer](../data_types/integer.md)       | `0`     | The height offset for where the leaves are made.
`leaf_height`      | [Integer](../data_types/integer.md)       | `3`     | The amount of leaves tall the tree is.
`chance_per_chunk` | [Integer](../data_types/integer.md)       | `33`    | the % chance of a tree appearing per chunk (0-100).

### Example Code

```json
{
    "type": "feature:tree",
    "log_block": "minecraft:quartz_pillar",
    "leaf_block": "minecraft:oak_leaves",
    "sapling_block": "minecraft:grass"
}
```
