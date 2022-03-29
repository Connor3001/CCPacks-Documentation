# Generic Particles

Type ID: `particle:generic`

### Fields

Field   | Type | Default | Description
-----------|------|---------|-------------
`colour` | [Colour](../data_types/colour.md) | `{"red": 1, "green": 1, "blue": 1, "alpha": 1)` | Determines the particles colour.
`size` | [Float](../data_types/float.md) | `0.25` | How large the particle is.
`max_age` | [Integer](../data_types/integer.md) | `100` | How long the particle will last for (in ticks).
`collides_with_world` | [Boolean](../data_types/boolean.md) | `false` | If set to true, the particle will have collisions.

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
