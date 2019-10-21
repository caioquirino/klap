# klap

zero config, zero dependency bundler for tiny javascript packages

[![Build Status](https://travis-ci.org/osdevisnot/klap.svg?branch=master)](https://travis-ci.org/osdevisnot/klap)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org/)

## Features

- **zero config**: detemine source and targets from `package.json`
- **zero config** typescript support: just rename `.js` file to `.ts`
- **tiny bundles**: produces tiny, optimized code for all inputs
- creates multiple output formats `cjs`, `umd` and `esm`
- **zero dependency**: uses bundled deps.

## Usage

First install klap as a global dep

```bash
npm install -g klap
```

Then, fire `init` command inside your package directory.

```bash
klap init
```

### `klap` commands

- Use **`npm run build`** to build your project.

- Use **`npm run watch`** to build and watch for changes.

- Use **`npm run start`** to watch and start a dev server.

## `klap` configuration

`klap` reads your `package.json` for config options. Notably,

- `pkg.source` determines source file to compile and bundle

- `pkg.main`, `pkg.module` and `pkg.browser` determines compilation targets

- `pkg.example` detemines the source file for `start` command

## License

**klap** is licensed under the [MIT License](http://opensource.org/licenses/MIT).

Documentation is licensed under [Creative Common License](http://creativecommons.org/licenses/by/4.0/).

Created with ♥ by [@osdevisnot](https://github.com/osdevisnot) and [all contributors](https://github.com/osdevisnot/klick/graphs/contributors).
