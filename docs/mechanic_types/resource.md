# Resource

[Mechanic Type](../mechanic_types.md).

Defines a resource for the block. Holds a persistent integer value, which can be modified by the [Change Resource](../entity_actions/change_stat.md) action and checked with the [Resource](../entity_conditions/check_stat.md) block condition.

Type ID: `ccpacks:resource`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`min` | [Integer](../data_types/integer.md) | 0 | The minimum value of the resource.
`max` | [Integer](../data_types/integer.md) | 1 | The maximum value of the resource.
`start_value` | [Integer](../data_types/integer.md) | 20 | The value of the resource when the block first gains this mechanic.

### Example
```json
{
    "type": "ccpacks:resource",
	"min": 0,
	"max": 100,
    "start_value": 20
}
```
This mechanic is a resource, which starts at a value of 20.
