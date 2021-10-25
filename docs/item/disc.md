# Custom Disc



### Fields

   Field   | Type | Default | Description
-----------|------|---------|-------------
`subtype` | [String]() | *mandatory* | Defines the type of item.
`identifier` | [Identifier]() | *mandatory* | The identifier is what the item appears as in the /give command.
`sound` | [Identifier]() | *mandatory* | the sound event that the disc uses.
`comparator_output` | [Int]() | *optional* | The signal strength a comparator outputs from this disc

### Example Code

```json
{
  "type": "item:music_disc",
  "comparator_output": 8,
  "sound": "example_pack:funky_sound"
}
```
