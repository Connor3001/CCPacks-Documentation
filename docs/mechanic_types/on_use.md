# On Use

[Mechanic Type](../mechanic_types.md).

A mechanic that is activated when a player interacts with the block.

Type ID: `ccpacks:on_use`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`block_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block when it is interacted with.
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | *optional* | The action to execute on the player when they interact with the block.
`block_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the block action.

### Example
```json
{
	"type": "ccpacks:on_use",
	"entity_action": {
		"type": "origins:heal",
		"amount": 6
	}
}
```
This mechanic will heal the player by 3 hearts when they interact with it.
