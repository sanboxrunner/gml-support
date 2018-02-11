# GML Support

![Version](https://vsmarketplacebadge.apphb.com/version/liaronce.gml-support.svg)
![Installs](https://vsmarketplacebadge.apphb.com/installs-short/liaronce.gml-support.svg)
![Rating](https://vsmarketplacebadge.apphb.com/rating/liaronce.gml-support.svg)

GameMaker Language Support in Visual Studio Code.

Visual Studio Code version should be higher than 1.8.0.

## Start

Search and install in Visual Studio Code, reload.

![](assets/sc1.png)

## Dependencies

This plug-in requires the [`vscode-icons`](https://github.com/vscode-icons/vscode-icons) and [`Shader languages support for VS Code`](https://github.com/stef-levesque/vscode-shader), these plug-ins will be installed automatically in this installation.

## Tasks

- [ ] Completing GameMaker:Studio's snippet (about 95% now).
- [ ] Completing GameMaker 8.1's snippet (about 85% now).
- [ ] Language Server.
- [ ] Debugger.

## Q&A

> 1, Why delete function information?

Because I think the effect of displaying function information on code snippets is very poor, I would like to implement it after I make a language server, I started to remove the function information in the code snippet from 1.3.3

## About GMLive

In 1.3.4, I add `GMLive` syntaxes, but I do not have this plugin, so it does not have any tests.

## Notices

The following functions are temporarily not added:

New in GameMaker 8.1:

draw_self() This command is exactly the same as draw_sprite_ext() except it will use the instances own variables to draw itself (x,y, scale, angle etc.) This provides the same action as if the instance was draw without a script.

get_function_address('function_name') Returns the address of a GameMaker function. This can be passed to DLL's so the can call directly into GameMaker.

.gmk and .gm81 file is GameMaker 8.1 project file! 
The file can not be edited by the text editor!
This is just to distinguish the GameMaker version.