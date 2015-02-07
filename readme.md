# Inexor Data Files

This repository contains all data for [Inexor](https://github.com/inexor-game/inexor).
It is intended as the core package, featuring up our main dependencies plus a few maps in ~300MB.
Anything else can get delivered via custom packages ingame.

## Licensing
A big problem we had to deal with when forking off Cube 2: Sauerbraten has been licensing.
This is why we decided to introduce a strict policy as you can find in [our wiki](https://github.com/inexor-game/data/wiki/License-Policy).


## How does the repo work?
The repo is splitted into packages, which may contain:
* maps
* textures
* sounds
* models
* and any additional content needed

A package will be documented using our package.json system - a example can be found below.
```json
{
    "title": "Package Title",
    "author": {
		"name": "Package Author",
		"email": "package@auth.or" 
	},
    "date": {
        "release": "package release date",
        "alpha": "package alpha date"
    },
    "license": "package license",
    "content": {
        "maps": [
            "package map"
        ],
        "textures": {
            "package texture folder": {
                "texture.png": "Some more detail about the texture",
                "moretexture.png": ""
            }
        },
        "models": {
            "package model folder": {
                "model.png": "Some more detail about the model",
                "moremodel.png": ""
            }
        },
        "dependencies": {
            "textures": [
                "texture1.png",
                "texture2.png"
            ],
            "skybox": [
                "skybox1.png"
            ]
		},
		"attribute": {
			"url": "http://some.pack.age",
			"credit": "this is a nice testing package made by a bear"
		}
    }
}

```
Don't let this frighten you, there will be a nice little GUI that takes care of writing the .json for you.


## How can I get involved / contribute?
Have a look in our [wiki](https://github.com/inexor-game/data/wiki/How-to-contribute-content).
