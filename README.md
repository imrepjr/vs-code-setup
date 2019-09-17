# VS Code setup

## Prettier & Visual Studio Code

How to set up Prettier with VS Code and elsint to autofix your code.

### VS code settings

Settings in [settings.json](./vscode-config/settings.json).

Relevant settings:

```JSON
{
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true,
    "[vue]": {
        "editor.formatOnSave": false
    },
    "eslint.validate": [
        "javascript",
        "javascriptreact",
        {
            "language": "vue",
            "autoFix": true
        }
    ],
    "eslint.autoFixOnSave": true,
    "prettier.printWidth": 120,
    "prettier.tabWidth": 4
}
```

## VS Code extensions

List of VS Code was removed, became deprecated with the [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) extension.

## Configure ESLint

ESLint config can be set up easily in `~` or in the root of the desired project folder in an `.eslintrc.json` file. Copy contents from the appropriate sample below.

Rule sets:

-   [vue.js](./general-vue-eslintrc.json)
-   [react](./react-eslintrc.json)

**TODO:**

-   Add `tslint` config!
