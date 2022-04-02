# Triggerable

[Mechanic Type](../mechanic_types.md).

Similar to [On Neighbour Update](on_neighbour_update.md) however, it is triggered by the [Trigger Mechanic](../block_actions/trigger_mechanic.md) block action.

Type ID: `ccpacks:triggerable`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`self_action` | [Block Action Type](https://apoli.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block.
`self_condition` | [Block Condition Type](https://apoli.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the self block action.
`neighbour_action` | [Block Action Type](https://apoli.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the neighbouring block.
`neighbour_condition` | [Block Condition Type](https://apoli.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the neighbouring block action.

### Example
```json
{
	"type": "ccpacks:triggerable",
	"self_action": {
		"type": "origins:spawn_entity",
		"command": "summon minecraft:item ~ ~1 ~ {Item:{id:\"minecraft:wheat\",Count:1}}"
	},
	"self_condition": {
		"type": "origins:light_level",
		"light_type": "block",
		"comparison": ">",
		"compare_to": 10
	}
}
```
This example  mechanic will summon a wheat item above the block once it is triggered if the block's light level is above 10.
