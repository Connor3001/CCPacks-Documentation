# Custom Stairs

### Fields

   Field           | Type | Default | Description
-------------------|------|---------|-------------
`material` | [Material](../block/materials.md) | *optional* | The sounds related to the player moving and walking on the block.
`effective_tool` | [Tool Type](../../data_types/tool_types) | *optional* | The tool you need to use to mine the block.
`block_sound_group` | [Block Sound Group](../block/sounds.md) | *optional* | The sounds related to the player moving and walking on the block.
`collidable` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *optional* | The sounds related to the player moving and walking on the block.
`transparent` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *optional* | The sounds related to the player moving and walking on the block.
`hardness` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *0.6f* | 
`resistance` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | The light level that the block gives off
`mining_level` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | What mining level you have to be in order to break the block.
`loot_table` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | null | *mandatory* | The loot table for the block(s) that is dropped when this block is broken
`make_block_item` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | true | If false, makes it so it does not register a block item.

### Example Code

```json
{
	"type": "block:stairs",
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
	"effective_tool": "pickaxes",
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
	"mining_level": 3,
	"loot_table": "example_pack:blocks/kunzite_stairs",
	"make_block_item": true,
	"item_group": "building_blocks"
}
```

This code makes a block that sounds like glass when broken, and when right clicked, opens a crafting GUI for the player