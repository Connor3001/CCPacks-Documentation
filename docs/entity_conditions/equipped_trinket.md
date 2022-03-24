# Equipped Trinket

Checks all the players trinket slots with an [Item Condition](https://origins.readthedocs.io/en/latest/types/item_condition_types/).

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_condition` | [Item Condition](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | *mandatory* | The items that are searched for in the trinket slots.

### Example
```json
"condition": {
  	"type": "ccpacks:equipped_trinket",
    "item_condition": {
        "type": "apoli:ingredient",
        "ingredient": {
            "item": "example_pack:kunzite_trinket"
        }
    }
}
```
Returns true if the player has the kunzite trinket equipped.
