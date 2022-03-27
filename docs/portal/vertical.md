# Vertical Dimension Portals

Type ID: `portal:vertical`

### Fields

  Field   | Type | Default | Description
-----------|------|---------|-------------
`block` | [Identifier](../data_types/identifier.md) | | The block that the portal is made out of.
`ignition_item` | [Identifier](../data_types/identifier.md) | `minecraft:flint_and_steel` | The item used to ignite the portal with.
`dimension` | [Identifier](../data_types/identifier.md) | `minecraft:the_end` | The dimension that the portal takes you to.
`colour` | [Colour Holder](../data_types/colour.md) | `{"red": 1, "green": 1, "blue": 1, "alpha": 1)` | The colour of the portal.

### Example Code

```json
{
	"type": "portal:vertical",
	"block": "minecraft:end_stone",
	"ignition_item": "minecraft:heart_of_the_sea",
	"dimension": "minecraft:the_end",
	"colour": {
		"red": 0.145,
		"green": 0.098,
		"blue": 0.2
	}
}
```
