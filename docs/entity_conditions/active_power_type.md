# Power Active

Checks whether the entity has a power that uses the specified [Power Type](https://origins.readthedocs.io/en/latest/types/power_types/), excluding those in the blacklist, and is "active", meaning that the entity has the power and the power has all its conditions fulfilled.

Type ID: `ccpacks:active_power_type`


### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`power_type` | [Identifier](../data_types/identifier.md) | *manditory* | The namespace ID of the power type which will be checked to see if any are active.
`blacklisted_powers` | [Array](../data_types/array.md) of [Identifier](../data_types/identifier.md) | *manditory* | The namespace IDs of powers that will be excluded from the check.


### Examples
```json
"condition": {
  	"type": "ccpacks:active_power_type",
      "power_type": "apoli:elytra_flight",
      "blacklisted_powers": [
          "example:elytra_power"
      ]
}
```
This will return true if the player has any elytra flight power that isnt "example:elytra_power".