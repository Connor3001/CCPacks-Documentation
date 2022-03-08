# Resource

[Power Type](../power_types.md).

Defines a stat bar for the player. Basically holds a persistent integer value between 0, and 20, which can be modified by the [Change Stat](../entity_actions/change_stat.md) action and checked with the [Check Stat](../entity_conditions/check_stat.md) player condition.

Type ID: `ccpacks:stat_bar`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`hud_render` | [Stat Bar Hud Render](../data_types/stat_hud_render.md) | | Specifies how and if the stat bar is displayed with a bar on the HUD.
`start_value` | [Integer](../data_types/integer.md) | 20 | The value of the resource when the player first gains this power.

### Example
```json
{
    "type": "ccpacks:stat_bar",
    "start_value": 20,
    "hud_render": {
        "should_render": true,
        "bar_index": 0,
        "side": "right",
        "sprite_location": "example_pack:textures/gui/icons.png"
    }
}
```
This power is a stat bar, which creates a bar of the given texture that is already completely filled.
