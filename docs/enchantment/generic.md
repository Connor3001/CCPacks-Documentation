# Enchantment

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`treasure` | [Boolean](../block/materials.md) | *required* | An Object that determines some behaviours of the block.
`target` | [Enchantment Target](../block/materials.md) | *breakable* | What type of item this will go on.
`max_level` | [Render Layer](../../data_types/tool_types) | *1* | The maximum level you can get with the enchantment.
`rarity` | [Block Sound Group](../block/sounds.md) | *very_rare* | Sets the rarity of the enchantment. Values: `common`, `uncommon`, `rare`, `very_rare`
`blacklist` | [List (Enchantment)](../submodules/apoli-docs/docs/data_types/boolean.md) | *optional* | A list of enchantments that you cannot have with this.

### Example Code

```json
{
	"type": "enchantment:generic"
}
```
