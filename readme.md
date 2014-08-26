# Sauerbraten Fork Data Files

This repository contains all data for [Sauerbraten Fork](https://github.com/sauerbraten-fork/sauerbraten-fork).
It is intended as the core package, featuring up our main depencies in a few ~100MB.

## Licensing
A big problem we had to deal with when forking off Sauerbraten has been licensing.
Due to imprecise licensing we were in need to throw all existing work aboard and take off.
This is why we decided to introduce a strict guideline as following
> All files in SauerFork may apply a license which grants full usage of the content (including commercial distribution)

You can find a list of licenses applying this terms below:

| License       | 
| ------------- | 
| [CC-0 1.0 or any later version](https://creativecommons.org/publicdomain/zero/1.0/)  | 
| [CC BY 3.0 or any later version](https://creativecommons.org/licenses/by-sa/3.0/)    |
| [CC BY-SA 3.0 or any later version](https://creativecommons.org/licenses/by-sa/3.0/) |
| [zlib](http://opensource.org/licenses/Zlib)                                          |
| [GPL](http://www.gnu.org/copyleft/gpl.html)                                          |
| [MIT](http://opensource.org/licenses/MIT)                                            |

## How does the repo work?
The repo is splitted into packages, which may contain:
* maps
* textures
* and any additional content needed

A package will be documented using our package.json system - a example can be found below.
```json
{
    "title": "Package Title",
    "author": "Package Author package@auth.or",
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
Don't let this frighten you, there is a nice little GUI that takes care of writing the .json for you.

~~Furthermore there is a folder for core scripts ( UI ) which will most certainly be replaced.~~ 

## How can I get involved / contribute
We're hiring anyone who want's to contribute!
Just get in contact with us, send a patch or open a issue and we'll take care of it..
