# Custom Trinkets

Custom Trinkets requires the [Trinkets](https://www.curseforge.com/minecraft/mc-mods/trinkets-fabric) mod in order to function. There is a [wiki for Trinkets](https://github.com/emilyalexandra/trinkets/wiki) that will help with getting trinkets set up.

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`item_group`| [Item Group](../../data_types/item_groups) | `misc` | The tab you can find the item in.
`name` | [String](../../data_types/string) | *optional* | Sets the items name.
`lore` | [String [array]](../submodules/apoli-docs/docs/data_types/string.md) | *optional* | Lines of text below an item.
`durability` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How many uses the item has.
`fuel_tick` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *optional* | How long the item can smelt for in a furnace.
`item_powers` | [Item Power [array]]() | *optional* | The powers your item will have.
`start_color` | [Color](data_types/color.md) | *optional* | How many uses the item has.
`end_color` | [Color](data_types/color.md) | *optional* | How many uses the item has.
`max_count` | [Integer](../submodules/apoli-docs/docs/data_types/integer.md) | *64* | The maximum stack count for the item.

### Example Code

```json
{
	"type": "item:trinket"
}
```
