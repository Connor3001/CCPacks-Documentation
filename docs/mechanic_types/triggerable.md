# Triggerable

[Mechanic Type](../mechanic_types.md).

Similar to [On Neighbour Update](on_neighbour_update.md) however, it is triggered by the [Trigger Mechanic](../block_actions/trigger_mechanic.md) block action.

Type ID: `ccpacks:triggerable`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`neighbour_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the neighbouring block.
`neighbour_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the neighbouring block action.
`self_action` | [Block Action Type](https://origins.readthedocs.io/en/latest/types/block_action_types/) | *optional* | The action to execute on the block.
`self_condition` | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | The condition to checked in order to run the self block action.

### Example
```json
{
	"type": "ccpacks:triggerable",
	"self_action": {
		"type": "origins:execute_command",
		"command": "summon minecraft:item ~ ~ ~ {Item:{id:\"minecraft:wheat\",Count:1}}"
	},
	"self_condition": {
		"type": "origins:light_level",
		"light_type": "block",
		"comparison": ">",
		"compare_to": 10
	}
}
```
This mechanic will summon the wheat item once triggered if the light is above 10.