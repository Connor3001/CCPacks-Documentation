# On Land

[Mechanic Type](../mechanic_types.md).

A Mechanic that is activated when a player falls onto the block

Type ID: `ccpacks:on_land`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`damage_multiplier` | [Float](../data_types/float.md) | 1.0 | Specifies how and if the stat bar is displayed with a bar on the HUD.
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | *optional* | The action to execute on the player when they land on the block.
`block_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block when it is landed on.
`block_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the block action.

### Example
```json
{
    "type": "ccpacks:on_land",
	"damage_multiplier": 0.0
}
```
This mechanic will create a block that negates all fall damage.