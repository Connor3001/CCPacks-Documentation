### Equipped Trinket

Checks all the players trinket slots with an [Item Condition]().

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_condition` | [Item Condition]() | *mandatory* | The identifier is what the sound appears as in the /playsound command.

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
