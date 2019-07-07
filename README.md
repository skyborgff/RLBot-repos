# RLBot repo donciderations

After some thinking i desided that multiple repolists would give us the abillity to offer solutions for all usecases. standard only the stableThrusted repo will be in the GUI, but for developers and testers there will be the option

the repo may contain one folder (the folder with the bot files, packaging.json added) github folders are allowed and will be ignored. files in the main folder will also be ignored.

# Syntax
```json
{
    "note": "Note when enabling the repo",
    "repos":[
        {
            "name": "should explain itself",
            "url": "https link to repo for download",
            "testedFrameworkVersion": "Latest framework version tested with, 0 if not tested or dev version",
            "testedVersion": "Latest bot version tested with, 0 if not tested or dev version or no version is known. this is also used to check for updates. if 0 user cannot be prompted of updates",
            "category": [
                {
                    "name": "name of bot categoty"
                }
            ],
            "gamemodes": [
                {
                    "name": "gamemodes supported in lowercase, short notation for 1v1, 2v2, 3v3 and 4v4"
                }
            ]
        }
    ]
}
```

# Example (stablerepo)
```json
{
    "note": "",
    "repos":[
        {
            "name": "RLbotPythonDataParser",
            "url": "https://github.com/ard1998/RLbotPythonDataParser.git",
            "testedFrameworkVersion": "1.20",
            "testedVersion": "1.0",
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
                }
            ] 
        }
    ]
}
```


# packaging.json
packaging.json is an slightly modified version of an repo entry. everything ouside the repos has veen cut out. testedVersion has veen replaced by botVersion below an example

```json
{
    "name": "RLbotPythonDataParser",
    "url": "https://github.com/ard1998/RLbotPythonDataParser.git",
    "testedFrameworkVersion": "1.20",
    "botVersion": "1.0",
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
        }
    ] 
}
```
