# Add own syntax highlighting(Testing)

In the current version I added highlighting support for some plugins, but I can not provide highlighting support for every plugins, so in 1.3.6 you can add your own highlight.

## How to add

 - Create an `extra.json` file in the `syntaxes` directory in the extension directory. e.g. `C:\Users\(your username)\.vscode\extensions\liaronce.gml-support-x.x.x\syntaxes`.

 - Writing and saving syntax highlighting in the following format.

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

 - Reloading Visual Studio Code