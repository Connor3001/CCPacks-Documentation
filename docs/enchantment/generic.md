# Enchantment

Type ID: `enchantment:generic`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`treasure` | [Boolean](../data_types/boolean.md) | `false` | If set to true, this enchantment won't appear on an Enchanting Table.
`target` | Enchantment Target (Undocumented) | `"breakable"` | What type of item this will go on.
`max_level` | [Integer](../data_types/integer.md) | `1` | The maximum level you can get with the enchantment.
`rarity` | [String](../data_types/string.md) | `"very_rare"` | Sets the rarity of the enchantment. Accepts `"common"`, `uncommon`, `rare` and `very_rare`
`blacklist` | [Array](../data_types/array.md) of [Identifiers](../data_types/identifier.md) | *optional* | A list of enchantments that you cannot have with this.

### Example Code

```json
{
	"type": "enchantment:generic"
}
```
