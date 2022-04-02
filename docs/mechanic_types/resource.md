# Resource

[Mechanic Type](../mechanic_types.md).

Defines a resource for the block. Holds a persistent integer value, which can be modified by the [Change Resource (Block Action Type)](../block_actions/change_resource.md) and checked with the [Resource (Block Condition Type)](../block_conditions/resource.md).

Type ID: `ccpacks:resource`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`min` | [Integer](../data_types/integer.md) | `0` | The minimum value of the resource.
`max` | [Integer](../data_types/integer.md) | `1` | The maximum value of the resource.
`start_value` | [Integer](../data_types/integer.md) | `0` | The value of the resource when the block first gains this mechanic.

### Example
```json
{
	"type": "ccpacks:resource",
	"min": 0,
	"max": 100,
	"start_value": 20
}
```
This example will create a resource with a minimum value of 0, maximum value of 1 and a starting value of 20.
