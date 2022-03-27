# Trigger Mechanic

!!! note
	This action will only work on CCPacks blocks with the [Triggerable (Mechanic Types)](../mechanic_types/triggerable.md) Mechanic.

Triggers a block's mechanic. Useful with the [Offset (Block Action Type)](https://origins.readthedocs.io/en/latest/types/block_action_types/offset/) meta action.

Type ID: `ccpacks:trigger_mechanic`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`mechanic` | [Identifier](../data_types/identifier.md) | *optional* | ID of the mechanic type that defines the resource. Must be a [Triggerable](../mechanic_types/triggerable.md) which exists on the block.

### Example
```json
"block_action": {
	"type": "ccpacks:trigger_mechanic",
	"mechanic": "example_pack:smelt"
}
```
triggers the `example_pack:smelt` mechanic on the block.
