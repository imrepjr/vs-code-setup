# VS Code setup

I created this repository to store my preferences related to Visual Studio Code
and to make them available for future reference for myself and anyone who
stumbles upon it. I plan on keeping it up-to-date whenever I find some new stuff
worth adding - suggestions, constructive comments are welcome.

## Prettier & Visual Studio Code

Here I have documented how I have set up the [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) extension
with VS Code and elsint to autofix your code and work along with other extensions
that provide automatic corrections.

### VS code settings

All of my settings can be found in [settings.json](./vscode-config/settings.json).

Below are the settings that I found relevant to make Prettier work without weird,
contradicting corrections alongside the Vetur extension and certain eslint
settings:

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

I removed the list of my VS Code extensions, it became deprecated (and I saw no
point in maintaining it) with the [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) extension.

## Configure ESLint

ESLint config can be set up easily in `~` or in the root of the desired project
folder in an `.eslintrc.json` file. Copy contents from the appropriate sample
below if you wish to try out my settings. More info on [ESLint in the official
docs](https://eslint.org/).

Rule sets:

-   [vue.js](./general-vue-eslintrc.json)
-   [react](./react-eslintrc.json)

**TODO:**

-   Add `tslint` config!
