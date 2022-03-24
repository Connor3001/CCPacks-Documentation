### Open Choice Screen

Opens the choice screen for the player, allowing for them to select a specific choice.

Type ID: `ccpacks:open_choice_screen`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`choice_layer` | [Identifier](../data_types/identifier.md) | *manditory* | ID of the choice layer that the action will open.

### Example
```json
"entity_action": {
  	"type": "ccpacks:open_choice_screen",
	"choice_layer": "example_pack:choice"
}
```
opens the `example_pack:choice` layer for the player.
