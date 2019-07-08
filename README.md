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
            "name": "RLbotPythonDataParser",
            "url": "https://github.com/ard1998/RLbotPythonDataParser/tree/repo-test"
        }
    ]
}

```


# packaging.json example
packaging.json is an slightly modified version of an repo entry. everything ouside the repos has been cut out. testedVersion has veen replaced by botVersion below an example. this file is to check updates and is to provide data for the local filter, so also unlisted packages can be filtered

```json
{
    "name": "RLbotPythonDataParser",
    "url": "https://github.com/ard1998/RLbotPythonDataParser/tree/repo-test",
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
        }
    ] 
}
```
