# Trigger Mechanic

[Block Action](../block_actions.md).

!!! note
	This action will only work on ccpacks blocks with the [Triggerable](../mechanic_types/triggerable.md) Mechanic.

Triggers a block's mechanic. Useful with the [Offset](https://origins.readthedocs.io/en/latest/types/block_action_types/offset/) meta action. 

Type ID: `ccpacks:trigger_mechanic`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`mechanic` | [Identifier](../data_types/identifier.md) |  | ID of the mechanic type that defines the resource. Must be a [Triggerable](../mechanic_types/triggerable.md) which exists on the block.

### Example
```json
"block_action": {
  	"type": "ccpacks:trigger_mechanic",
	"mechanic": "example_pack:smelt"
}
```
triggers the `example_pack:smelt` mechanic on the block.
