# Custom Trinkets

Custom Trinkets requires the [Trinkets](https://www.curseforge.com/minecraft/mc-mods/trinkets-fabric) mod in order to function. There is a [wiki for Trinkets](https://github.com/emilyalexandra/trinkets/wiki) that will help with getting trinkets set up.

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`durability` | [Integer]() | *mandatory* | How many uses the item has.

### Example Code

```json
{
	"type": "item:trinket"
}
```
