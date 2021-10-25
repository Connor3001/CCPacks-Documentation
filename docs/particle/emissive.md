# Particles

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`color` | [Color](data_types/color.md) | *mandatory* | The identifier is what the particle appears as in the /particle command.
`size` | [Float](../submodules/apoli-docs/docs/data_types/float.md) | *mandatory* | does the particle glow?
`max_age` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *mandatory* | does the particle glow?
`collides_with_world` | [Boolean](../submodules/apoli-docs/docs/data_types/boolean.md) | *mandatory* | does the particle glow?

### Example Code

```json
{
	"type": "particle:emissive",
	"color": {
		"red": 1,
		"blue": 1,
		"green": 0
	}
}
```
