### Universal Powers

Custom Content Packs allow you to use the same power system as origins (Apoli), with your custom content for greater variety. In order to use the universal power system. you make your power files as you would in origins. And then make the directories `/data/<namespace>/universal_powers/` and create a json file in there (it can be named anything)
Then, in this file, you enter your powers, and entities, as shown in the following examples:

### Examples
```
{
	"powers": [
		"namespace:power_name",
		"namespace:power_name_2"
	],
	"entity_entry": {
		"entity": "minecraft:player"
	}
}
```
This example would apply the powers `namespace:power_name` and `namespace:power_name_2` to all players.

```
{
	"powers": [
		"namespace:power_name",
		"namespace:power_name_2"
	],
	"entity_entry": {
		"tag": "minecraft:skeletons"
	}
}
```
This example would apply the powers `namespace:power_name` and `namespace:power_name_2` to all entities in the tag `minecraft:skeletons`.