# Color

[Data Type](../data_types.md).

An [Object](object.md) used to define how a stat bar should be rendered.

### Fields:

Field  |      Type         | Default | Description
-------|-------------------|---------|-------------
`red`  | [Float](../data_types/float.md) | 1.0 | Value by which the red component of the texture will be multiplied. Range: 0 - 1
`green`| [Float](../data_types/float.md) | 1.0 | Value by which the green component of the texture will be multiplied. Range: 0 - 1
`blue` | [Float](../data_types/float.md) | 1.0 | Value by which the blue component of the texture will be multiplied. Range: 0 - 1
`alpha`| [Float](../data_types/float.md) | 1.0 | Value by which the alpha (= transparency) component of the texture will be multiplied. Range: 0 - 1

### Examples:

```json
"color": {
	"red": 1,
	"green": 0,
	"blue": 0
}
```

This definition results in a red color.
<br>

```json
"color": {
	"red": 0,
	"green": 0,
	"blue": 1,
	"alpha": 0.5
}
```

This definition results in a slightly transparent blue color