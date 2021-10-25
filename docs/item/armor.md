# Custom Armor

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`name` | [String]() | *mandatory* | The name of the image files used to texture the armor.
`durability` | [Integer]() | *10* | How many uses the item has.
`protection` | [Integer]() | *0* | the amount of damage that a weapon does.
`knockback_resistance` | [Integer]() | *0* | How fast you can swing the weapon.
`enchantability` | [Integer]() | *0* | How likely you are to get good enchantments.
`lore` | [String [array]]() | *optional* | Lines of text below an item.
`repair_item` | [Item]() | *optional* | The item used to repair the armour.

### Armor json structure

```json
{
	"type": "item:armor",
	"slot": "chest",
	"name": "kunzite",
	"durability": 750,
	"protection": 5,
	"toughness": 1,
	"knockback_resistance": 0,
	"enchantability": 6,
	"item_group": "materials"
}
```
