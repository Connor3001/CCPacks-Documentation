# Item Group

Type ID: `item_group:generic`

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`icon` | [Identifier](../data_types/identifier.md) | | The item that the tab will use for the icon.
`items` | [Array](../data_types/identifier.md) of [Identifier](../data_types/identifier.md) | *optional* | The items that are in the Item Group.

### Example Code

```json
{
    "type": "item_group:generic",
    "icon": "example_pack:drill_slime_block",
    "items": [
        "example_pack:chorus_slime_block",
        "example_pack:drill_slime_block",
        "example_pack:explosive_slime_block",
        "example_pack:magma_slime_block",
        "example_pack:crafting_slime_block"
    ]
}
```
