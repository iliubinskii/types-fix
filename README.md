# Types Fix

[![Version](https://img.shields.io/github/package-json/v/ilyub/types-fix)](https://github.com/ilyub/types-fix)
[![Downloads](https://img.shields.io/npm/dm/types-fix)](https://www.npmjs.com/package/types-fix)
[![Source rank](https://img.shields.io/librariesio/sourcerank/npm/types-fix)](https://libraries.io/npm/types-fix)
[![Dependencies](https://img.shields.io/librariesio/release/npm/types-fix)](https://libraries.io/npm/types-fix)
[![Vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/types-fix)](https://snyk.io/advisor/npm-package/types-fix)

## Table of contents

- [Overview](#overview)
- [Typescript any-to-unknown](#typescript-any-to-unknown)

## <a name="overview"></a>Overview

This package fixes some global types (currently it contains one fix &mdash; see below).

Installation:
```sh
npm install --save-dev types-fix
```

## <a name="typescript"></a>Typescript any-to-unknown

This fix replaces _any_ with _unknown_ in some typescript types.
Use it for better type checking in your project.

```ts
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
