### Trigger Mechanic

[Block Action](../block_actions.md).

Triggers a neighbouring block's mechanic. *Only works on `ccpacks:triggerable` mechanics*

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
