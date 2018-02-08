# GML Support

![Version](https://vsmarketplacebadge.apphb.com/version/liaronce.gml-support.svg)
![Installs](https://vsmarketplacebadge.apphb.com/installs-short/liaronce.gml-support.svg)
![Rating](https://vsmarketplacebadge.apphb.com/rating/liaronce.gml-support.svg)

GameMaker Language 对 Visual Studio Code 的支持。

Visual Studio Code版本需高于1.8.0。

## 开始

在 Visual Studio Code 中直接搜索安装，重新加载即可。

![](../assets/sc1.png)

## 依赖

本插件需要 [`vscode-icons`](https://github.com/vscode-icons/vscode-icons) 和 [`Shader languages support for VS Code`](https://github.com/stef-levesque/vscode-shader)，这些将在本插件安装时自动安装。

## 任务

* [ ] 完善 GameMaker:Studio 的代码片段（现在完成大约 75% ）
* [ ] 完善 GameMaker 8.1 的代码片段（现在完成大约 10% ）
* [ ] Language Server
* [ ] 调试器

## Q&A

> 1, 为什么移除了函数信息

因为我认为在代码片段上显示函数信息的效果很不好，我想在制作出语言服务器之后再进行实现，所以从 1.3.3 开始移除代码片段中的函数信息。