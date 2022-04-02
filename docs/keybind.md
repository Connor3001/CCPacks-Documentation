# Keybinds

Type ID: `keybind:apoli`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`name` | [String](data_types/string.md) | *optional* | The name of the keybind, it is used in powers.
`category` | [String](data_types/string.md) | *optional* | The name of the keybind, keybinds with the same category will be grouped together.

### Example Code

```json
{
	"type": "keybind:apoli",
	"name": "winged_boost",
	"category": "example_pack_keybinds"
}
```

This example would create a keybind with the ID `key.ccpacks.winged_boost`, which would appear in the Keybind category `example_pack_keybinds`.
