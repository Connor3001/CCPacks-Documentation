# Change Resource

[Block Action](../block_actions.md).

!!! note
	This action will only work on ccpacks blocks with the [Resource](../mechanic_types/resource.md) Mechanic.

Type ID: `ccpacks:change_resource`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`resource` | [Identifier](../data_types/identifier.md) |  | ID of the mechanic type that defines the resource. Must be a [Resource](../mechanic_types/resource.md) which exists on the block.
`change` | [Integer](../data_types/integer.md) |  | This value will be added to the resource.
`operation` | [String](../data_types/string.md) | "add" | Determines if the action should add or set the value of the resource. Accepts `"add"` or `"set"`.

### Example
```json
"block_action": {
    "type": "ccpacks:change_resource",
    "resource": "example_pack:fuel",
    "change": 1,
	"operation": add
}
```
This action adds 1 to the `example_pack:fuel` [resource](../power_types/resource.md) power. (`data\example_pack\mechanics\fuel.json`)