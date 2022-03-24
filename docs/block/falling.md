# Falling Block

Type ID: `block:falling`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`material` | [Material](../data_types/materials.md) | *manditory* | An Object that determines some behaviours of the block.
`mechanics` | [Array](../data_types/array.md) of [Mechanic Type](../mechanic_types.md) | *optional* | A list of [Mechanic Type](../mechanic_types.md) that the block will have.
`render_layer` | [Render Layer](../data_types/render_layer.md) | *Solid* | The blocks render layer `ewsagsfv`.
`block_sound_group` | [Block Sound Group](../data_types/sounds.md) | *optional* | The sounds related to the player moving and walking on the block.
`collidable` | [Boolean](../data_types/boolean.md) | *true* | Wether you can walk through the block or not
`transparent` | [Boolean](../data_types/boolean.md) | *false* | Sets the block to be `nonOpaque`.
`hardness` | [Integer](../data_types/integer.md) | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float](../data_types/float.md) | *0.6f* | How slippery the block is to walk on.
`resistance` | [Integer](../data_types/integer.md) | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer](../data_types/integer.md) | *0* | The light level that the block gives off.
`mining_level` | [Integer](../data_types/integer.md) | *1* | What mining level you have to be in order to break the block.
`loot_table` | [Identifier](../data_types/identifier.md) | *optional* | The loot table for the block that is dropped when this block is broken.
`block_item` | [Block Item](../data_types/block_item.md) | *optional* | An object for creating an item for the block.

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
	"block_item": {
		"name": "Gravel Ore",
		"item_group": "building_blocks"
	}
}
```