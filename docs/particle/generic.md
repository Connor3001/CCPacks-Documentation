# Particles

Type ID: `particle:generic`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`colour` | [Colour](../data_types/colour.md) | (1,1,1,1) | Determines the particles colour.
`size` | [Float](../data_types/float.md) | 0.25 | How large the particle is.
`max_age` | [Integer](../data_types/integer.md) | 100 | How long the particle last for (in ticks).
`collides_with_world` | [Boolean](../data_types/boolean.md) | false | Does the particle collide with the world?

### Example Code

```json
{
	"type": "particle:generic",
	"color": {
		"red": 1,
		"blue": 1,
		"green": 0
	}
}
```
