# Falling Block

Falling blocks are identical to generic blocks, but they are affected by gravity.

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`material` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`effective_tool` | [Effective Tool]() | *optional* | The tool you need to use to mine the block.
`block_sound_group` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`collidable` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`transparent` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`hardness` | [Integer]() | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float]() | *0.6f* | 
`resistance` | [Integer]() | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer]() | *0* | The light level that the block gives off
`mining_level` | [Integer]() | *optional* | What mining level you have to be in order to break the block.
`loot_table` | [Loot Table]() | null | *mandatory* | The loot table for the block(s) that is dropped when this block is broken
`make_block_item` | [Boolean]() | true | If false, makes it so it does not register a block item.

### Example Code

```json
{
	"type": "block:falling",
	"material": {
		"allow_light": false,
		"allow_movement": true,
		"blocks_pistons": false,
		"burnable": false,
		"destroyed_by_piston": false,
		"liquid": false,
		"not_solid": false,
		"replaceable": false
	},
	"effective_tool": "shovels",
	"block_sound_group": {
		"pitch": 1,
		"volume": 1,
		"break_sound": "block.gravel.break",
		"step_sound": "block.gravel.step",
		"place_sound": "block.gravel.place",
		"hit_sound": "block.gravel.hit",
		"fall_sound": "block.gravel.fall"
	},
	"collidable": true,
	"transparent": false,
	"hardness": 3,
	"slipperiness": 0.6,
	"resistance": 3,
	"luminance": 0,
	"mining_level": 2,
	"loot_table": "example_pack:blocks/kunzite_ore_gravel",
	"make_block_item": true,
	"item_group": "building_blocks"
}
```