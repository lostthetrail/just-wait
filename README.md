# just-wait

[![version](https://img.shields.io/npm/v/just-wait.svg)](https://npmjs.org/package/just-wait) ![license](https://img.shields.io/npm/l/just-wait.svg) ![installs](https://img.shields.io/npm/dt/just-wait.svg)

Waits for a file or directory to change or appear, then just returns. The watched file or directory does not have to exist yet.

Based off of [Rick Wong](https://github.com/RickWong)'s [wait-run](https://www.npmjs.com/package/wait-run),
this simplified version just waits for the file or directory to appear/change and then returns. It does not
execute any commands.

## Installation

```bash
npm install --g just-wait
```

## Usage

```bash
just-wait --pattern '*.*' && say hello    # waits for any change in cwd then runs once.
```

## License

BSD 3-Clause license. Copyright © 2016, Rick Wong. All rights reserved.
