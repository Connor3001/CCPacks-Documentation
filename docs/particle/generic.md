# Particles

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`identifier` | [Identifier]() | *mandatory* | The identifier is what the particle appears as in the /particle command.
`glowing` | [Bool]() | *mandatory* | does the particle glow?

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
