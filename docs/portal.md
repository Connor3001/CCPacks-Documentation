# Dimension Portals

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`block` | [Identifier]() | *mandatory* | The block that the portal is made out of.
`ignition_item` | [Identifier]() | *mandatory* | The Item used to ignite the portal with.
`dimension` | [Identifier]() | *mandatory* | The dimension that the portal takes you to.
`color` | [Color]() | *optional* | The red value of the portal.

### Example Code

```json
{
	"type": "portal:vertical",
	"block": "minecraft:end_stone",
	"ignition_item": "minecraft:heart_of_the_sea",
	"dimension": "minecraft:the_end",
	"color": {
		"red": 37,
		"green": 25,
		"blue": 51
	}
}
```
