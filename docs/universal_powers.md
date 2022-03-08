### Universal Powers

Custom Content Packs allow you to use the same power system as origins (Apoli), with your custom content for greater variety. In order to use the universal power system. you make your power files as you would in origins. And then make the directories `/data/<namespace>/universal_powers/` and create a json file in there (it can be named anything)
Then, in this file, you enter the following, replacing the power names with your repective powers.
```
{
	"powers": [
		"namespace:power_name",
		"namespace:power_name_2"
	],
	"entity_condition": {
		"type": "apoli:entity_type",
		"entity_type": "minecraft:creeper"
	}
}
```
