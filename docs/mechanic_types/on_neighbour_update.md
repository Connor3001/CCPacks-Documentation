# On Neighbour Update

[Mechanic Type](../mechanic_types.md).

A Mechanic that is run when this block is updated (e.g. a block being placed next to it).

Type ID: `ccpacks:on_neighbour_update`

!!! note
		This Mechanic type is called `on_neighbour_update`, not `on_neighbor_update`!

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`self_action` | [Block Action Type](https://apoli.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block.
`neighbour_action` | [Block Action Type](https://apoli.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the neighbouring block.
`self_condition` | [Block Condition Type](https://apoli.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the self block action.
`neighbour_condition` | [Block Condition Type](https://apoli.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the neighbouring block action.

### Example
```json
{
	"type": "ccpacks:on_neighbour_update",
	"self_action": {
		"type": "origins:execute_command",
		"command": "summon minecraft:zombie"
	},
	"neighbour_condition": {
		"type": "origins:block",
		"block": "minecraft:diamond_block"
	}
}
```
This mechanic will summon a zombie if a diamond block is placed next to this block.
