# 添加自定义语法高亮（测试）

在目前的版本中我添加了部分插件的语法高亮支持，但我不可能对每一个插件都提供语法高亮支持，所以在 1.3.6 中加入了自定义语法高亮，你可以自行添加。

这是一个测试性的功能，我也欢迎你贡献其他插件的语法。

## How to add

 - 在插件目录的`syntaxes`文件夹内创建一个`extra.json`文件。 例如 `C:\Users\(your username)\.vscode\extensions\liaronce.gml-support-x.x.x\syntaxes`.

 - 按照以下格式书写并保存。

```json
{
	"$schema": "https://raw.githubusercontent.com/martinring/tmlanguage/master/tmlanguage.json",
    "fileTypes": ["gml"],
    "scopeName": "source.gml-extra",
	  "patterns": [
      {
         "match": "(?i)\\b(liaronce_test)\\b",
         "name": "support.function.gml-extra"
      },
      {
         "match": "(?i)\\b(liaronce_test)\\b",
         "name": "constant.gml-extra"
      },
      {
         "match": "(?i)\\b(liaronce_test)\\b",
         "name": "support.variable.gml-extra"
      }
   ]
}
```

 - 重新加载 Visual Studio Code