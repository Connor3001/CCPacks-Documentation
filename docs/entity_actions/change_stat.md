# Change Stat

Changes the value of a [Star Bar](../power_types/stat_bar.md).

Type ID: `ccpacks:change_stat`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`stat_bar` | [Identifier](../data_types/identifier.md) | *manditory* | ID of the power type that defines the stat bar. Must be a [Stat Bar](../power_types/stat_bar.md) which exists on the player.
`change` | [Integer](../data_types/integer.md) | *manditory* | This value will be added to the resource (won't go below 0 or above 20).
`operation` | [String](../data_types/string.md) | "add" | Determines if the action should add or set the value of the resource. Accepts `"add"` or `"set"`.

### Example
```json
"entity_action": {
    "type": "ccpacks:change_stat",
    "stat_bar": "example_pack:mana_bar",
    "change": 1
}
```
This action adds 1 to the `example_pack:mana_bar` [Stat Bar](../power_types/stat_bar.md) power. (`data\namespace\powers\example.json`)