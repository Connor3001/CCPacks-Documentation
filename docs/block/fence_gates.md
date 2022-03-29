# Fence Gate Block

Type ID: `block:fence_gate`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`material` | [Material](../data_types/materials.md) | | An Object that determines some behaviours of the block.
`mechanics` | [Array](../data_types/array.md) of [Identifiers](../data_types/identifier.md) | *optional* | The namespace and IDs of the Block Mechanics this block will have.
`render_layer` | [Render Layer](../data_types/render_layer.md) | `"solid"` | The blocks render layer `ewsagsfv`.
`block_sound_group` | [Block Sound Group](../data_types/sounds.md) | *optional* | The sounds related to the player moving and walking on the block.
`collidable` | [Boolean](../data_types/boolean.md) | `true` | Whether you can walk through the block or not
`transparent` | [Boolean](../data_types/boolean.md) | `false` | If set to true, makes the block `nonOpaque`.
`hardness` | [Integer](../data_types/integer.md) | `3` | How long the block takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float](../data_types/float.md) | `0.6` | How slippery the block is to walk on.
`resistance` | [Integer](../data_types/integer.md) | `3` | Short for "Blast Resistance". Defines how resistant to explosions the block will be (3 is stone, 1500 is obsidian).
`luminance` | [Integer](../data_types/integer.md) | `0` | The light level that the block gives off.
`requires_tool` | [boolean](../data_types/boolean.md) | `false` | If set to true, the block will require a specific tool to be broken.
`loot_table` | [Identifier](../data_types/identifier.md) | *optional* | The loot table that the block uses to define what to drop when broken.
`block_item` | [Block Item](../items/generic.md) | *optional* | An object for creating an item for the block.

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
