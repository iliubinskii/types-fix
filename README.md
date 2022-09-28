# Types Fix

[![Stars](https://img.shields.io/github/stars/ilyub/types-fix)](https://github.com/ilyub/types-fix)
[![Downloads](https://img.shields.io/npm/dm/types-fix)](https://www.npmjs.com/package/types-fix)
[![Vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/types-fix)](https://snyk.io/advisor/npm-package/types-fix)
[![Dependencies](https://img.shields.io/librariesio/release/npm/types-fix)](https://libraries.io/npm/types-fix)

## Table of contents

- [Overview](#overview)
- [Installation](#installation)
- [TypeScript any-to-unknown](#typescript-any-to-unknown)
- [Related packages](#related-packages)

## <a id="overview"></a>Overview

This package fixes some global types (currently it contains one fix &mdash; see below).

## <a id="installation"></a>Installation

```sh
npm install --save-dev types-fix
```

## <a id="typescript-any-to-unknown"></a>TypeScript any-to-unknown

This fix replaces _any_ with _unknown_ in some TypeScript core types.
Use it for better type checking.

### Configuration

```jsonc
// tsconfig.json
{
  "compilerOptions": {
    "typeRoots": [
      "node_modules/@types",
      "node_modules/types-fix"
    ],
    "types": [
      "typescript-any-to-unknown"
    ]
  }
}
```

## <a id="related-packages"></a>Related packages

- [eslint-plugin-misc](https://www.npmjs.com/package/eslint-plugin-misc) &mdash; ESLint plugin.
- [quasar-extension](https://www.npmjs.com/package/quasar-extension) &mdash; Quasar extension.
- [real-fns](https://www.npmjs.com/package/real-fns) &mdash; A collection of utility functions.
- [real-classes](https://www.npmjs.com/package/real-classes) &mdash; A collection of utility classes.
- [real-facades](https://www.npmjs.com/package/real-facades) &mdash; Facades (each facade provides interface to pluggable implementation).
- [real-service-providers](https://www.npmjs.com/package/real-service-providers) &mdash; Facade implementations.
