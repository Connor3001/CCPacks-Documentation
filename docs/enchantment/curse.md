# Curse

Type ID: `enchantment:curse`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`treasure` | [Boolean](../data_types/boolean.md) | false | Is this enchantment considered treasure?
`target` | [Enchantment Target](../data_types/enchantment_target.md) | *breakable* | What type of item this will go on.
`max_level` | [Render Layer](../data_types/render_layer.md) | *1* | The maximum level you can get with the enchantment.
`rarity` | [Rarity](../data_types/rarity.md) | *very_rare* | Sets the rarity of the enchantment. Values: `common`, `uncommon`, `rare`, `very_rare`
`blacklist` | [Array](../data_types/array.md) od [Identifier](../data_types/identifier.md) | *optional* | A list of enchantments that you cannot have with this.

### Example Code

```json
{
	"type": "enchantment:curse"
}
```
