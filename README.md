# Turborepo Mui Sandbox

## Installation

```sh
pnpm dlx create-turbo@latest
```

```sh
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/package.json`
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/tsconfig.json`
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/src/index.ts`
```

```sh
pnpm add @mui/material@5.8.7 @mui/styled-engine @mui/styled-engine-sc@^5.8.0 styled-components@5.3.6 -F @repo/mui
```

## pnpm patch

Modify packages/mui/node_modules/@mui/material/index.js:

```sh
pnpm patch @mui/material
```

Open `'/private/var/folders/95/xf7tpy6x10x90w2r865z51x80000gn/T/4d17ea785f89b6e9006210c58edce3ef'`, edit and save.
Then:

```js
/** @license MUI v5.8.7
 *
 * This source code is licensed under the MIT license found in the
 * LICENSE file in the root directory of this source tree.
 */
/**
 * Add a comment to check pnpm patch
 */
/* eslint-disable import/export */
```

```sh
pnpm patch-commit '/private/var/folders/95/xf7tpy6x10x90w2r865z51x80000gn/T/4d17ea785f89b6e9006210c58edce3ef'
```
