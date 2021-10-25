# Custom Food

### Fields:

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`max_count` | [Integer]() | *64* | How many of the item you can have in one stack.
`hunger` | [Integer]() | *4* | how many hunger it fills up (1 = half a bar)
`saturation` | [Float]() | *8f* | How many saturation points the food fills
`meat` | [Boolean]() | *false* | Can it be fed to dogs?
`always_edible` | [Boolean]() | *false* | Can you eat it even when full?
`returns` | [Item]() | *false* | The item that this item returns when used.
`drinkable` | [Boolean]() | *false* | If true, makes you drink it as apposed to eating.
`sound` | [Sound]() | *false* | The sound you play while you are eating it
`eating_time` | [Integer]() | *false* | The amount of time (in ticks) it takes to eat
`eat_action` | [Entity Action]() | *false* | The action to run when it is eaten.
`lore` | [String [array]]() | *optional* | Lines of text below an item.

### Example Code:

```json
{
    "type": "item:food",
    "max_count": 64,
    "hunger": 8,
    "saturation": 12,
    "meat": false,
    "always_edible": true,
    "returns": "minecraft:diamond",
    "drinkable": false,
    "sound": "minecraft:block.sand.place",
    "eating_time": 60
}
```
