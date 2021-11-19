# Color

[Data Type](../data_types.md).

An [Object](object.md) used to define how a stat bar should be rendered.

### Fields:

####Item Powers:

Field  |      Type         | Default | Description
-------|-------------------|---------|-------------
`power`  | [Power](../data_types/float.md) | *mandetory* | The ID for the power to grant.
`slot`| [Equipment Slot](../data_types/float.md) | "mainhand" | The slot that power is active in.
`hidden` | [Boolean](../data_types/float.md) | false | Wether the item shows that it has this power.
`negative`| [Boolean](../data_types/float.md) | false | Changes wether the tooltip is blue, or red.

####Trinket Powers:

Field  |      Type         | Default | Description
-------|-------------------|---------|-------------
`power`  | [Power](../data_types/float.md) | *mandetory* | The ID for the power to grant.
`hidden` | [Boolean](../data_types/float.md) | false | Wether the item shows that it has this power.
`negative`| [Boolean](../data_types/float.md) | false | Changes wether the tooltip is blue, or red.

### Examples:

```json
"item_powers": [
	{
		"power": "example_pack:use_staff"
	},
	{
		"power": "example_pack:use_staff_2"
	}
]
```

This is 2 different powers, that will be visible on the items tooltip, and function in the main hand.
