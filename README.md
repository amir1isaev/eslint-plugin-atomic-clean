![GitHub CI](https://github.com/amir1isaev/eslint-plugin-atomic-clean/actions/workflows/ci.yml/badge.svg)
[![npm version](https://badge.fury.io/js/eslint-plugin-atomic-clean.svg?v=0.2.4)](https://badge.fury.io/js/eslint-plugin-atomic-clean)
[![HitCount](https://hits.dwyl.com/amir1isaev/eslint-plugin-atomic-clean.svg?style=flat-square)](http://hits.dwyl.com/amir1isaev/eslint-plugin-atomic-clean)

# eslint-plugin-atomic-clean

A comprehensive linting solution that sweeps your code clean. Fly through your codebase with ease and precision!

## Table of Contents

<!-- toc -->

- [Installation](#installation)
- [Usage](#usage)

<!-- tocstop -->

### Installation

You'll first need to install [ESLint](https://eslint.org/):

```sh
npm i eslint --save-dev
npm i typescript
```

Next, install `eslint-plugin-atomic-clean`:

```sh
npm install eslint-plugin-atomic-clean --save-dev
```

Next, install all peerDependencies for this plugin:

```sh
npx install-peerdeps eslint-plugin-atomic-clean
```

### Usage

Add `atomic-clean` to the extends or plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaVersion": 13,
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true,
      "modules": true,
      "experimentalObjectRestSpread": true
    }
  },
  "ignorePatterns": [
    "**/*",
    "node_modules"
  ],
  "settings": {
    "react": {
      "pragma": "React",
      "fragment": "Fragment",
      "version": "detect"
    },
    "import/resolver": {
      "typescript": {
        "alwaysTryTypes": true
      }
    }
  },
  "extends": [
    "plugin:atomic-clean/recommended"
  ],
  "plugins": [
    "atomic-clean"
  ]
}
```