# Custom Tools

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`durability` | [Integer]() | *10* | How many uses the item has.
`mining_speed_multiplier` | [Float]() | *0* | (unknown, if you know, tell me on the discord)
`attack_damage` | [Integer]() | *0* | the amount of damage that a weapon does.
`attack_speed` | [Integer]() | *0* | How fast you can swing the weapon.
`mining_level` | [Integer]() | *optional* | doesn't actually do anything on swords.
`enchantability` | [Integer]() | *0* | How likely you are to get good enchantments.
`lore` | [String [array]]() | *optional* | Lines of text below an item.

### Example Code

```json
{
    "type": "item:axe",
    "durability": 450,
    "mining_speed_multiplier": 10,
    "attack_damage": 11,
    "attack_speed": 1.1,
    "mining_level": 4,
    "enchantability": 12,
    "lore": [
        "a fragile tool and weapon"
    ]
}
```
