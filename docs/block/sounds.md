# Block Sound Group

[Data Type](../data_types.md).

An [Object](object.md) used to define what sounds a block should make

### Fields:

Field                |                  Type               |  Default  | Description
---------------------|-------------------------------------|-----------|-------------
`pitch`              | [Sound](../data_types/sound.md)     |     1     | Allow light to pass through the block.
`volume`             | [Sound](../data_types/sound.md)     |     1     | <-->
`break_sound`        | [Sound](../data_types/sound.md)     |*manditory*| <-->
`step_sound`         | [Sound](../data_types/sound.md)     |*manditory*| <-->
`place_sound`        | [Sound](../data_types/sound.md)     |*manditory*| <-->
`hit_sound`          | [Sound](../data_types/sound.md)     |*manditory*| <-->
`fall_sound`         | [Sound](../data_types/sound.md)     |*manditory*| <-->

### Examples:

```json
"block_sound_group": {
	"pitch": 1,
	"volume": 1,
	"break_sound": "block.gravel.break",
	"step_sound": "block.gravel.step",
	"place_sound": "block.gravel.place",
	"hit_sound": "block.gravel.hit",
	"fall_sound": "block.gravel.fall"
}
```