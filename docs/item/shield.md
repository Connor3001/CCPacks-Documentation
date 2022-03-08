# Custom Shield

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`item_powers` | [Item Power [array]]() | *optional* | The powers your item will have.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`cooldown` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *60* | How long the shield takes to be able to be used again when struck with an axe.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *100* | How many uses the item has.
`enchantability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *0* | How likely you are to get good enchantments.
`repair_item` | [Identifier](../submodules/apoli-docs/docs/data_types/identifier.md) | *optional* | The item used to repair this item.

### Example Code

```json
{
    "type": "item:shield",
    "cooldown": 20,
    "durability": 100,
    "enchantability": 9
}
```
