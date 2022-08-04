# Code editor



### Editor <a href="#editor" id="editor"></a>

We prefer to use [Visual Studio Code](https://code.visualstudio.com/) as our editor

The following plugins are recommended:

* Code Spell Checker
* GitLens
* Import Cost
* Prettier
* Better comments
* Eslint

The following plugins are nice-to-have:

* Color Highlight
* Path Intellisense
* vscode-icons
* Jest Runner
* vscode-styled-components
* Auto Rename Tag

These settings can also come in handy (`.vscode/settings.json`)

```
{
  "editor.tabSize": 2,
  "editor.formatOnSave": true,
  "workbench.iconTheme": "vscode-icons",
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "tslint.autoFixOnSave": true,
  "cSpell.userWords": ["backend", "fibricheck", "qompium"],
  "typescript.updateImportsOnFileMove.enabled": "always"
}
```
