# Dimension Portals

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`block` | [Identifier](../data_types/identifier.md) | *mandatory* | The block that the portal is made out of.
`ignition_item` | [Identifier](../data_types/identifier.md) | `minecraft:flint_and_steel` | The item used to ignite the portal with.
`dimension` | [Identifier](../data_types/identifier.md) | `minecraft:the_end` | The dimension that the portal takes you to.
`colour` | [Colour Holder](../data_types/colour.md) | (1,1,1,1) | The colour of the portal.

### Example Code

```json
{
	"type": "portal:horizontal",
	"block": "minecraft:end_stone",
	"ignition_item": "minecraft:heart_of_the_sea",
	"dimension": "minecraft:the_end",
	"colour": {
		"red": 37,
		"green": 25,
		"blue": 51
	}
}
```
