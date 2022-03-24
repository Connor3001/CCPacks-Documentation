# Power Active

Checks whether the entity has a power that uses the speciifed [Power Type](), excluding those in the blacklist, and is "active", meaning that the entity has the power and the power has all its conditions fulfilled.

Type ID: `origins:active_power_type`


### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`power_type` | [Identifier](../data_types/identifier.md) | *manditory* | The namespace ID of the power type which will be checked to see if any are active.
`blacklisted_powers` | [Array](../data_types/array.md) of [Identifier](../data_types/identifier.md) | *manditory* | The namespace IDs of powers that will be excluded from the check.


### Examples
