# Item Use

[Power Type](../power_types.md).

This power uses the existing item interaction system in Minecraft to execute actions. which means that when used, the actions won't happen if something of higher priority occurs (for example opening a chest).

Type ID: `ccpacks:item_use`

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`cooldown` | [Integer](../data_types/integer.md) | `0` | Sets a cooldown on the item (Similar to ender pearl cooldowns).
`entity_action` | [Entity Action Type](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | _optional_ | The entity action to be executed on the player if specified.
`item_action` | [Item Action Type](https://origins.readthedocs.io/en/latest/types/item_action_types/) | _optional_ | The item action to be executed if specified.
`item_condition` | [Item Condition Type](https://origins.readthedocs.io/en/latest/types/item_condition_types/) | _optional_ | If specified, only execute the action if the item condition is fulfilled.

### Example
```json
{
	"type": "ccpacks:item_use",
	"cooldown": 20,
	"item_action": {
		"type": "apoli:damage",
		"amount": 1
	},
	"item_condition": {
		"type": "ccpacks:compare_durability",
		"comparison": ">",
		"compare_to": 1
	},
	"entity_action": {
		"type": "ccpacks:change_stat",
		"stat_bar": "example_pack:mana_bar",
		"change": -2
	},
	"condition": {
		"type": "ccpacks:check_stat",
		"stat_bar": "example_pack:mana_bar",
		"comparison": ">=",
		"compare_to": 2
	}
}
```

This power is in the example pack, attached to the `kunzite_staff`. When the item is used, it damages the item, if its durability is greater than 1. and it also removes from the players mana, if that is also not empty.
