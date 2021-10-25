### Compare Durability

Checks the durability of a certain item.

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`comparison` | [Comparison]() | |  In what way to compare the durability the specified value.
`compare_to` | [Integer]() | | The value to compare durability against.

### Example

```json
"item_condition": {
    "type": "ccpacks:compare_durability",
    "comparison": ">",
    "compare_to": 0
}
```
Checks if the item has more than 0 durability.