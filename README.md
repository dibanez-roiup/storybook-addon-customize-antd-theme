<div align="center">

[![GitHub license](https://img.shields.io/github/license/pocka/storybook-addon-designs.svg)](https://github.com/pocka/storybook-addon-designs/blob/master/LICENSE)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

</div>

<hr/>

## storybook-addon-customize-antd-theme

A [Storybook](https://github.com/storybooks/storybook) addon that visually customize an ant design theme in the addon panel for better design-development workflow.

- [Docs & Demo](https://letshare.github.io/storybook-addon-customize-antd-theme)

## Requirements

- Storybook@>=6.0.0

This addon should work well with any framework: If you find the case the addon not works, please open an issue.

## Getting started

### 1. Install

```sh
npm install --D storybook-addon-customize-antd-theme
# yarn add -D storybook-addon-customize-antd-theme
```

### 2. Register the addon in `main.js`

```js
module.exports = {
  stories: ['storybook-addon-customize-antd-theme/dist/esm/stories/index.js'],
  addons: ['storybook-addon-customize-antd-theme'],
};
```

### 3. Setting default story states

You can initial setup ant design theme, by setting the `customizeAntdTheme` property on `parameters`:

```js
// .storybook/preview.js

export const parameters = {
  customizeAntdTheme: {
    modifyVars: {
      'primary-color': '#ff1771',
      'border-radius-base': '20px',
    },
  },
};
```
