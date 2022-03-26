# Bind Item

[Power Type](../power_types.md).

Makes certain items unable to leave in the entity's inventory until death.

Type ID: `ccpacks:bind_item`

### Fields

Field | Type | Default | Description
------|------|---------|------------
`item_condition` | [Item Condition Type](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | _optional_ | If specified, only make the items that fulfill the specified item condition type are unable to leave the players inventory.
`slots` | [Array](../data_types/array.md) of [Integers](../data_types/integer.md) | _optional_ | If specified, only make the items that are in the listed inventory slots are unable to leave the players inventory. See [Positioned Item Stack Slots](https://origins.readthedocs.io/en/latest/misc/extras/positioned_item_stack_slots/) for possible values.

### Example