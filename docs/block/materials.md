# Materials

[Data Type](../data_types.md).

An [Object](object.md) used to define the properties of the block.

### Fields:

Field                |                  Type               | Default | Description
---------------------|-------------------------------------|---------|-------------
`liquid`             | [Boolean](../data_types/boolean.md) |  false  | <Not yet documented, if discovered please let me know on the discord>
`solid`          	 | [Boolean](../data_types/boolean.md) |  true   | <Not yet documented, if discovered please let me know on the discord>
`blocks_movement`    | [Boolean](../data_types/boolean.md) |  true   | Stops the player from walking through the block.
`blocks_light`       | [Boolean](../data_types/boolean.md) |  true   | Stops light from going through the block.
`burnable`           | [Boolean](../data_types/boolean.md) |  false  | determines whether the block burns.
`piston_behaviour`	 | [Boolean](../data_types/boolean.md) | `normal`| <Not yet documented, if discovered please let me know on the discord> Values: `normal`, `destroy`, `block`, `ignore`, `push_only`

### Examples:

```json
"material": {
	"allow_light": false,
	"allow_movement": true,
	"blocks_pistons": false,
	"burnable": false,
	"destroyed_by_piston": false,
	"liquid": false,
	"not_solid": false,
	"replaceable": false
}
```