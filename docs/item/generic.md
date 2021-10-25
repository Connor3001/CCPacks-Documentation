# Custom Items

### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`max_count` | [Integer]() | *1* | How many uses the item has.
`lore` | [String [array]]() | *optional* | Lines of text below an item.

### Example Code

```json
{
	"type": "item:generic",
	"item_group": "materials",
	"max_count": 64
}
```
