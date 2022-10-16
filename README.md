# VS Code setup

I created this repository to store my preferences related to Visual Studio Code
and to make them available for future reference for myself and anyone who
stumbles upon it. I plan on keeping it up-to-date whenever I find some new stuff
worth adding - suggestions, constructive comments are welcome.

## Fonts

- [FiraCode](https://github.com/tonsky/FiraCode)

## Prettier & Visual Studio Code

Here I have documented how I have set up the [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) extension
with VS Code and elsint to autofix your code and work along with other extensions
that provide automatic corrections.

### VS code settings

All of my settings can be found in [settings.json](./vscode-config/settings.json).

## VS Code extensions

TODO

## Configure ESLint

ESLint config can be set up easily in `~` or in the root of the desired project
folder in an `.eslintrc.json` file. Copy contents from the appropriate sample
below if you wish to try out my settings. More info on [ESLint in the official
docs](https://eslint.org/).

Rule sets:

-   [vue.js](./general-vue-eslintrc.json)
-   [react](./react-eslintrc.json)
