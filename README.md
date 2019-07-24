# RLBot repo

After some thinking i desided that multiple repolists would give us the abillity to offer solutions for all usecases. standard only the stableThrusted repo will be in the GUI, but for developers and testers there will be the option

the content of the download folder in the head of the repo will be cloned to the bot folder

# Syntax
```json
{
	"note": "Note when enabling the repo",
	"repos":[
		{
			"name": "name of botfolder",
			"url": "link to the branch. best practice: make an repo for each version",
			"testedFrameworkVersion": "tested version of the framework",
			"version": "version name",
			"category": [
				{
					"name": "Category name"
				},
				{...}
			],
			"gamemodes": [
				{
					"name": "gamemode name"
				}
				{...}
			] 
		}
	]
}
```

# repo example
```json
{
	"note": "",
	"repos":[
		{
			"name": "dataParse",
			"url": "https://github.com/ard1998/RLbotPythonDataParser",
			"branch": "repo-test",
			"testedFrameworkVersion": "1.20",
			"version": "1.0",
			"category": [
				{
					"name": "Example"
				},
				{
					"name": "Simple"
				}
			],
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
			] 
		}
	]
}

```


# packaging.json
packaging.json contains the info about the bot and will be used for local filtering. it is eaqual to an entity of the repo array of the repo file


# packaging.json example
```json
{
	"name": "dataParse",
	"url": "https://github.com/ard1998/RLbotPythonDataParser",
	"branch": "repo-test",
	"testedFrameworkVersion": "1.20",
	"version": "1.0",
	"category": [
		{
			"name": "Example"
		},
		{
			"name": "Simple"
		}
	],
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
	] 
}
```
