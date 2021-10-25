# Action On Being Used

[Power Type](../power_types.md)

Executes an Entity Action and a Block Action at the location that a thrown projectile lands.

Type ID: `ccpacks:action_on_projectile_land`

### Fields

Field | Type | Default | Description
------|------|---------|-------------
`entity_action` | [Entity Action](../submodules/apoli-docs/docs/entity_actions.md) | _optional_ | The entity action to be executed if specified.
`block_action` | [Block Action](../submodules/apoli-docs/docs/block_actions.md) | _optional_ | The block action to be executed if specified.
`block_condition` | [Block Condition](../submodules/apoli-docs/docs/block_conditions.md) | _optional_ | If specified, only execute the specified actions if the block condition is fulfilled.

### Example
```json
{
    "type": "apoli:action_on_projectile_land",
    "block_action": {
		"type": "apoli:set_block",
		"block": "minecraft:diamond_block"
	},
    "block_condition": {
        "type": "apoli:block",
		"block": "minecraft:coal_block"
    }
}
```
This example enables other players to steal diamonds from the player that has the power.