# On Step

[Mechanic Type](../mechanic_types.md).

A Mechanic that is activated when a player walks on the block.

Type ID: `ccpacks:on_step`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | *optional* | The action to execute on the player when they step on the block.
`block_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block when it is stepped on.
`block_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the block action.

### Example
