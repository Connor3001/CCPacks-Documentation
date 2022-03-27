# Item Projectile

Type ID: `projectile:item`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`damage` | [Integer](../data_types/integer.md) | `0` | The damage that the projectile will deal.
`height` | [Float](../data_types/float.md) | `0.25` | The height of the projectile.
`width` | [Float](../data_types/float.md) | `0.25` | The width of the projectile.
`gravity` | [Float](../data_types/float.md) | `0.03` | The gravity that the projectile will have.
`base_item` | [Identifier](../data_types/identifier.md) | | The item that the projectile will look like.
`damage_source` | [Damage Source](../data_types/damage_source.md) | | The damage source that the projectile deals.

### Example Code

```json
{
	"type": "projectile:item",
	"damage": 4,
	"base_item": "minecraft:magenta_dye",
	"damage_source": {
		"name": "staff",
		"magic": true
	}
}
```
