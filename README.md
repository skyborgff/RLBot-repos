# RLBot repo

repo files, syntax, examples and instruction for interacting with or developing (for) the hub of rlbot 

## Syntax
```json
{
	"note": "Note when enabling the repo",
	"repos":[
		{
			"name": "name of botfolder",
			"url": "link to the branch. best practice: make an repo for each version",
			"branch": "branch of the repo"
		}
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
			"url": "https://github.com/ard1998/RLbotPythonDataParser",
			"branch": "repo-test"
		}
	]
}
```

## packaging.json syntax
```json
{
	"name": "name of botfolder",
	"url": "link to the branch. best practice: make an repo for each version",
	"branch": "branch of the repo",
	"version": "version name",
	"testedFrameworkVersion": "framework verion the bot is tested with",
	"version": "version of the bot",
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
```


## packaging.json example
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
