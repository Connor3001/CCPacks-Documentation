# Item Projectile

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`damage` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *mandatory* | The block that the portal is made out of.
`height` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *mandatory* | The Item used to ignite the portal with.
`width` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *mandatory* | The dimension that the portal takes you to.
`base_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The red value of the portal.
`damage_source` | [Damage Source](../submodules/apoli-docs/docs/misc/vanilla_damage_sources.md) | *optional* | The red value of the portal.

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
