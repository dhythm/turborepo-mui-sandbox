# Turborepo Mui Sandbox

## Installation

```sh
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/package.json`
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/tsconfig.json`
sh -c 'mkdir -p "$(dirname "$0")" && touch "$0"' `echo packages/mui/src/index.ts`
```

```sh
pnpm add @mui/material@5.8.7 @mui/styled-engine @mui/styled-engine-sc@^5.8.0 styled-components@5.3.6 -F @repo/mui
```
