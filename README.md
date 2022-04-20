# @btrya/eslint-config

[![npm](https://img.shields.io/npm/v/@btrya/eslint-config?color=00bfff&label=)](https://npmjs.com/package/@btrya/eslint-config)

## Usage

### Install

```bash
# all
npm install @btrya/eslint-config --save-dev
# for JS
npm install @btrya/eslint-config-basic --save-dev
# for TS
npm install @btrya/eslint-config-ts --save-dev
# for Vue + TS
npm install @btrya/eslint-config-vue --save-dev
# for React + TS
npm install @btrya/eslint-config-react --save-dev
```

### Config `.eslintrc`

```json
{
  "extends": "@btrya"
}
# or for single module
{
  "extends": "@btrya/eslint-config-basic"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```
