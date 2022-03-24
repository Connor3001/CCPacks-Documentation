# Choice JSON Format

This is the format of a JSON file describing a choice. They need to be placed inside the `choices` folder within your namespace.

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`powers` | [Array](../docs/data_types/array.md) of [Identifiers](../docs/data_types/identifier.md) | _optional_ | IDs of the powers this choice should have.
`icon` | [Item Stack](../docs/data_types/item_stack.md) | _optional_ | The item stack which is displayed as the icon for the description button for the choice
`name` | [String](../docs/data_types/string.md) | _optional_ | The display name of the choice.
`description` | [String](../docs/data_types/string.md) | _optional_ | The description of the choice.
`action_on_chosen` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | _optional_ | The description of the choice.

### Example

```json
{
    "powers": [
        "example_pack:mana_bar",
        "example_pack:mana_recharge",
        "example_pack:mana_recharge_2"
    ],
    "icon": "minecraft:diamond",
    "name": "Magic User",
    "description": "You can harness mana to use in a staff!"
}
```
This example choice adds  with a `minecraft:diamond` as its icon.
