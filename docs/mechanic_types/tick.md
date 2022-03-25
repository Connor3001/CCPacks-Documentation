# Tick

[Mechanic Type](../mechanic_types.md).

A Mechanic that is run every x ticks.

Type ID: `ccpacks:tick`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`interval` | [Integer](../data_types/integer.md) | 1 | Interval of ticks between subsequent executions of the specified actions. Must be a value of at least 1.
`block_action` | [Block Action Types](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block that has the power each interval.
`block_condition` | [Block Condition Types](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the block action.

### Example
