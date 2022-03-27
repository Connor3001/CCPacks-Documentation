# Item Powers

[Data Type](../data_types.md).

An [Object](object.md) which defines a power granted by an item.


### Fields

## Regular Item Powers

Field  | Type | Default | Description
-------|------|---------|-------------
`power` | [Identifier](identifier.md) | | ID of a Power.
`slot` | [Slot](integer.md) | `"mainhand"` | Slot that the power is granted for.
`hidden` | [Boolean](boolean.md) | `false` | Is the power visible on the item.
`negative` | [Boolean](boolean.md) | `false` | Is the power a negative power.

## Trinket Item Powers

Field  | Type | Default | Description
-------|------|---------|-------------
`power` | [Identifier](identifier.md) | | ID of a Power.
`hidden` | [Boolean](boolean.md) | `false` | Is the power visible on the item.
`negative` | [Boolean](boolean.md) | `false` | Is the power a negative power.


### Examples

```json
"item_powers": [
	{
		"power": "example_pack:wand",
		"slot": "mainhand"
	},
	{
		"power": "example_pack:wand",
		"slot": "offhand"
	}
]
```
Grants the power `example_pack:wand` when in either the `mainhand`, or `offhand` slot.
