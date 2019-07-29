# RLBot repo

repo files, syntax, examples and instruction for interacting with or developing (for) the hub of rlbot 

## Syntax
```json
{
	"note": "Note when enabling the repo",
	"repos":[
		{
			"name": "name of botfolder",
			"url": "link to the branch or repo (if bot is in master)"
		},
		{...}
	]
}
```

## repo example
```json
{
	"note": "",
	"repos":[
		{
			"name": "dataParse",
			"url": "https://github.com/ard1998/RLbotPythonDataParser"
		}
	]
}
```

## botpackage.json syntax
```json
{
	"name": "name of botfolder",
	"description": "bot description",
	"version": "version name, if not equal to the installed version the hub shows an update is available",
	"testedFrameworkVersion": "framework verion the bot is tested with",
	"botLanguage": "programing language the bot is written in",
	"gamemodes": [
		{
			"name": "gamemode name"
		}
		{...}
	],
	"categories": [
		{
			"name": "Category name"
		},
		{...}
	]
}
```


## botpackage.json example
```json
{
	"name": "dataParse",
	"description": "dev example with parsed structure",
	"version": "1.0",
	"testedFrameworkVersion": "1.20",
	"botLanguage": "python",
	"gamemodes": [
		{
			"name": "1v1"
		},
		{
			"name": "2v2"
		},
		{
			"name": "3v3"
		},
		{
			"name": "4v4"
		},
		{
			"name": "snowday"
		}
	],
	"categories": [
		{
			"name": "Example"
		},
		{
			"name": "Simple"
		}
	]
}
```
