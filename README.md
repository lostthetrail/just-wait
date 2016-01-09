# just-wait

[![version](https://img.shields.io/npm/v/just-wait.svg)](https://npmjs.org/package/just-wait) ![license](https://img.shields.io/npm/l/just-wait.svg) ![installs](https://img.shields.io/npm/dt/just-wait.svg)

Waits for a file or directory to change or appear, then just returns. The watched file or directory does not have to exist yet.

Based off of [Rick Wong](https://github.com/RickWong)'s [wait-run](https://www.npmjs.com/package/wait-run),
this simplified version just waits for the file or directory to appear/change and then returns. It does not
execute any commands. Use it by chaining commands after it using `&&`, which works under *nix as well as Windows.

Credits also go to [Fabian Eichenberger](https://github.com/queckezz), who created [watch-run](https://github.com/queckezz/watch-run), 
which was the basis for Rick's version.


## Installation

```bash
npm install --g just-wait
```

## Usage

```bash
# wait for changes in the current working dir before proceeding with the next command
just-wait --pattern '*.*' && echo Done!

# Proceed with the next command after an extra delay of 500ms
just-wait --pattern '*.*' --delay 500 && echo Done!

# Timeout after 10 seconds
just-wait --pattern '*.*' --timeout 10 && echo Done!
```

## Copyright 
* © 2016, [Stijn de Witt](http://StijnDeWitt.com). (this project)
* © 2016, [Rick Wong](https://github.com/RickWong). (wait-run)
* © 2015, [Fabian Eichenberger](https://github.com/queckezz). (watch-run)

## License
* [Creative Commons Attribution 4.0 (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/) (this project)
* [BSD 3-Clause license](https://opensource.org/licenses/BSD-3-Clause) (wait-run)
* [MIT License](https://opensource.org/licenses/MIT) (watch-run)
