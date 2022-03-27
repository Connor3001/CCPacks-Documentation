# Neutral Status Effect

Type ID: `"status_effect:neutral"`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
colour` | [Colour Holder](../data_types/colour.md) | `{"red": 1, "green": 1, "blue": 1, "alpha": 1)` | The colours used in the status effect's particles. The alpha value doesn't affect this.

Add functionality using [Power Types](https://origins.readthedocs.io/en/latest/types/power_types/) and [Universal Powers](../universal_powers.md)

### Example Code

```json
{
	"type": "status_effect:neutral",
	"colour": {
		"red": 1,
		"green": 1,
		"blue": 1
	}
}
```
