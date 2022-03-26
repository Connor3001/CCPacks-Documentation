# Resource

!!! note
	This condition will only work on ccpacks blocks with the [Resource](../mechanic_types/resource.md) Mechanic.

Checks the value of a power that uses the [Resource (Mechanic Type)](../mechanic_types/resource.md).

Type ID: `ccpacks:resource`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`resource` | [Identifier](../data_types/identifier.md) | *manditory* | The namespace ID of a mechanic that will be evaluated.
`comparison` | [Comparison](../data_types/comparison.md) | "==" | How the value of the mechanic that will be evaluated should be compared to the specified value.
`compare_to` | [Integer](../data_types/integer.md) | 0 | The value to compare the value of the mechanic that will be evaluated to.

### Example
```json
"block_condition": {
    "type": "ccpacks:resource",
	"resource": "example:resource",
	"comparison": ">=",
	"compare_to": 1
}
```