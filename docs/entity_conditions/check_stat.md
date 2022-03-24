# Check Stat

[Entity Condition](../entity_conditions.md).

Checks the value of a [Star Bar](../power_types/stat_bar.md).

Type ID: `ccpacks:check_stat`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`stat_bar` | [Identifier](../data_types/identifier.md) | *manditory* | ID of the power type that defines the stat bar. Must be a [Stat Bar](../power_types/stat_bar.md) which exists on the player.
`comparison` | [Comparison](https://origins.readthedocs.io/en/latest/types/data_types/comparison/) | "==" | How the value of the power that will be evaluated should be compared to the specified value.
`compare_to` | [Integer](../data_types/integer.md) | 0 | The value to compare the value of the power that will be evaluated to.

### Example
```json
"entity_action": {
    "type": "ccpacks:check_stat",
    "stat_bar": "example_pack:mana_bar",
    "comparison": ">",
	"compare_to": 0
}
```
This condition checks to see if `example_pack:mana_bar` [Stat Bar](../power_types/stat_bar.md) has a value greater than 0. (`data\namespace\powers\example.json`)