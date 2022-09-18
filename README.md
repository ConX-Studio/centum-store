# Centum Store Data - How to use
## Gamepasses
To find out which gamepass an item is you can copy the ID (ex: 71409714) and replace GAMEPASSID in this link:

https://www.roblox.com/game-pass/GAMEPASSID/info
### Marking an item as "on sale"
To make an item appear as on sale you need to set the "OriginalPrice" property of a gamepass.

Example, before:
```json
	"71409714": {
		"Tools": [
			{
				"Name": "Glock-17"
			}
		]
	},
```

Example, after:
```json
	"71409714": {
		"OriginalPrice": 1000,
		"Tools": [
			{
				"Name": "Glock-17"
			}
		]
	},
```

The store page will automatically be updated to show the old "OriginalPrice" and the new price (the new price is gotten from the price on Roblox).