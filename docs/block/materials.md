# Materials

[Data Type](../data_types.md).

An [Object](object.md) used to define how a stat bar should be rendered.

### Fields:

Field                |                  Type               | Default | Description
---------------------|-------------------------------------|---------|-------------
`allow_light`        | [Boolean](../data_types/boolean.md) |  false  | Allow light to pass through the block.
`allow_movement`     | [Boolean](../data_types/boolean.md) |  false  | <-->
`blocks_pistons`     | [Boolean](../data_types/boolean.md) |  false  | <-->
`burnable`           | [Boolean](../data_types/boolean.md) |  false  | <-->
`destroyed_by_piston`| [Boolean](../data_types/boolean.md) |  false  | <-->
`liquid`             | [Boolean](../data_types/boolean.md) |  false  | <-->
`not_solid`          | [Boolean](../data_types/boolean.md) |  false  | <-->
`replaceable`        | [Boolean](../data_types/boolean.md) |  false  | <-->

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