# Block Sound Group

[Data Type](../data_types.md).

An [Object](object.md) used to define what sounds a block should make

### Fields:

Field                |          Type               |  Default  | Description
---------------------|-----------------------------|-----------|-------------
`pitch`              | [Integer](integer.md)       |    `1`    | Sets the pitch of the sound.
`volume`             | [Integer](integer.md)       |    `1`    | Sets the volume
`break_sound`        | [Identifier](identifier.md) |           | The sound that plays when you break the block.
`step_sound`         | [Identifier](identifier.md) |           | The sound that plays when you step on the block.
`place_sound`        | [Identifier](identifier.md) |           | The sound that plays when you place the block.
`hit_sound`          | [Identifier](identifier.md) |           | The sound that plays when you hit the block.
`fall_sound`         | [Identifier](identifier.md) |           | The sound that plays when you fall on the block.

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
