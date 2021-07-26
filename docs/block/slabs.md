# Custom Slabs

There are two types of slabs, vertical, and horizontal. these are specified by using `ccpacks:horizontal_slab` and `ccpacks:vertical_slab`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of block
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`sound` | [Sound]() | *1* | The sound the block makes when broken.
`material` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`effective_tool` | [Effective Tool]() | *optional* | The tool you need to use to mine the block.
`mining_level` | [Integer]() | *optional* | What mining level you have to be in order to break the block.
`hardness` | [Integer]() | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float]() | *0.6f* | 
`resistance` | [Integer]() | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer]() | *0* | The light level that the block gives off
`loot_table` | [Loot Table]() | null | *mandatory* | The loot table for the block(s) that is dropped when this block is broken

### Example Code

```json
{
	"type": "ccpacks:block",
	"subtype": "horizontal_slab",
	"identifier": "example_pack:emerald_block",
	"sound": "glass",
	"material": "stone",
	"effective_tool": "pickaxe",
	"mining_level": 2,
	"hardness": 3,
	"slipperiness": 0.6,
	"resistance": 3,
	"luminance": 15,
    "loot_table": "example_pack:data",
	"action": {
		"type": "ccpacks:crafting_gui"
	}
}
```

This code makes a block that sounds like glass when broken, and when right clicked, opens a crafting GUI for the player