# Web3Studio ESlint Config

A collection of boilerplate config to be used by Web3Studio javascript based projects.

## Installation

```bash
$ yarn add --dev eslint-config-web3studio eslint prettier pretty-quick husky
```

In your `.eslintrc.js` file:

```js
module.exports = {
  extends: ['web3studio']
};
```

In your `.prettierrc.js` file:

```js
module.exports = require('eslint-config-web3studio/prettier');
```

In your `package.json` file:

```json
{
  "husky": {
    "hooks": {
      "pre-commit": "pretty-quick --staged"
    }
  },
  "scripts": {
    "lint": "eslint .",
    "prettier": "prettier \"**/*.{js,json,css,md}\" --write"
  }
}
```
