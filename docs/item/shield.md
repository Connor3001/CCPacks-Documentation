# Custom Shield

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`cooldown` | [Integer]() | *60* | How long the shield takes to be able to be used again when struck with an axe.
`durability` | [Integer]() | *100* | How many uses the item has.
`enchantability` | [Integer]() | *0* | How likely you are to get good enchantments.
`lore` | [String [array]]() | *optional* | Lines of text below an item.

### Example Code

```json
{
    "type": "item:shield",
    "cooldown": 20,
    "durability": 100,
    "enchantability": 9
}
```
