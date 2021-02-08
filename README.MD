[npm]: https://img.shields.io/npm/v/vite-logger
[npm-url]: https://www.npmjs.com/package/vite-logger
[size]: https://packagephobia.now.sh/badge?p=vite-logger
[size-url]: https://packagephobia.now.sh/result?p=vite-logger

# vite-logger

[![npm][npm]][npm-url]
[![size][size]][size-url]

unified vite plugin’s logger fork from vite.

## Usage

- run `yarn add vite-logger --dev`

```ts
import { createLogger } from 'vite-logger';
import chalk from 'chalk';

const logger = createLogger('info', true);

logger.warn(
  chalk.yellow.bold(
    `this is a warn message only print with logLevel >= 'warn' ` +
      `and can also mixed by chalk`
  )
)
```

## Options

### `level`

Type: `'error' | 'warn' | 'info' | 'silent'`<br>
Default: `silent`

### `allowClearScreen`

Type: `Boolean`<br>
Default: `false`
