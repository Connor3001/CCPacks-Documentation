# Fence Gate Block

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`material` | [Material](../block/materials.md) | *required* | An Object that determines some behaviours of the block.
`mechanics` | [List (Mechanic)](../block/materials.md) | *optional* | A list of [Mechanics]() that the block will have.
`render_layer` | [Render Layer](../../data_types/tool_types) | *Solid* | The blocks render layer `ewsagsfv`.
`block_sound_group` | [Block Sound Group](../block/sounds.md) | *optional* | The sounds related to the player moving and walking on the block.
`collidable` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *true* | Wether you can walk through the block or not
`transparent` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *false* | Sets the block to be `nonOpaque`.
`hardness` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *0.6f* | 
`resistance` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | The light level that the block gives off.
`mining_level` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *1* | What mining level you have to be in order to break the block.
`loot_table` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The loot table for the block that is dropped when this block is broken.
`block_item` | [Block Item](../submodules/apoli-docs/docs/data_types/boolean.md) | true | An object for creating an item for the block.

### Example Code

```json
{
	"type": "block:fence_gate",
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
	"loot_table": "example_pack:blocks/kunzite_fence_gate",
	"block_item": {
		"name": "Gravel Ore",
		"item_group": "building_blocks"
	}
}
```
