# Custom Stairs

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`sound` | [Sound]() | *1* | The sound the block makes when broken.
`material` | [Material]() | *optional* | The sounds related to the player moving and walking on the block.
`effective_tool` | [Effective Tool]() | *optional* | The tool you need to use to mine the block.
`mining_level` | [Integer]() | *optional* | What mining level you have to be in order to break the block.
`hardness` | [Integer]() | *3* | How long it takes to break (3 is stone 50 is obsidian).
`slipperiness` | [Float]() | *0.6f* | 
`resistance` | [Integer]() | *3* | How immune to explosions the block is (3 is stone, 1500 is obsidian).
`luminance` | [Integer]() | *0* | The light level that the block gives off
`loot_table` | [Identifier]() | *optional* | The loot table that the block drops when mined. Mines nothing if left behind.
`base_block` | [Identifier]() | *mandatory* | The block that the stairs are based on (determines properties of the block).
`make_block_item` | [Boolean]() | true | If false, makes it so it does not register a block item.
`loot_table` | [Loot Table]() | null | *mandatory* | The loot table for the block(s) that is dropped when this block is broken

### Example Code

```json
{
    "type": "block:stairs",
    "sound": "glass",
    "material": "stone",
    "effective_tool": "pickaxe",
    "mining_level": 2,
    "hardness": 3,
    "slipperiness": 0.989,
    "resistance": 3,
    "luminance": 15,
	"loot_table": "example_pack:data",
	"base_block": "minecraft:ice"
}
```

This code makes a block that sounds like glass when broken, and when right clicked, opens a crafting GUI for the player