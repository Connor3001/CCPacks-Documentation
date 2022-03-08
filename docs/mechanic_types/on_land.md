# Stat Bar

[Mechanic Type](../mechanic_types.md).

Defines a stat bar for the player. Basically holds a persistent integer value between 0, and 20, which can be modified by the [Change Stat](../entity_actions/change_stat.md) action and checked with the [Check Stat](../entity_conditions/check_stat.md) player condition.

Type ID: `ccpacks:on_land`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`damage_multiplier` | [Float](../data_types/float.md) | 1.0 | Specifies how and if the stat bar is displayed with a bar on the HUD.
`entity_action` | [Stat Bar Hud Render](../data_types/entity_action.md) | _optional_ | Specifies how and if the stat bar is displayed with a bar on the HUD.
`block_action` | [Stat Bar Hud Render](../data_types/block_action.md) | _optional_ | Specifies how and if the stat bar is displayed with a bar on the HUD.
`block_condition` | [Integer](../data_types/block_condition.md) | _optional_ | The value of the resource when the player first gains this power.

### Example
```json
{
    "type": "ccpacks:on_land",
	"damage_multiplier": 0.0
}
```
This mechanic will create a block that negates all fall damage.