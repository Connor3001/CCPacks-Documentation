### Compare Durability

Checks the durability of a certain item.

Type ID: `ccpacks:compare_durability`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`comparison` | [Comparison](https://origins.readthedocs.io/en/latest/types/data_types/comparison/) | "==" |  In what way to compare the durability the specified value.
`compare_to` | [Integer](../data_types/integer.md) | 0 | The value to compare durability against.

### Example

```json
"item_condition": {
    "type": "ccpacks:compare_durability",
    "comparison": ">",
    "compare_to": 0
}
```
Checks if the item has more than 0 durability.