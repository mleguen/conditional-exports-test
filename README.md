# Conditional exports test

Demonstrates that, with conditional exports, a single module can publish commonjs and ESM entrypoints,
both using the same typescript compiled modules.

## Installation

```bash
cd hello-world
npm pack
cd ../test-hello-world
npm install
```

## Usage

From `test-hello-world` directory:

```bash
$ node index.js
Hello World!
$ node --experimental-modules index.mjs
Hello World!
```

> **Note**: the `--experimental-modules` flag is not required with nodejs >= 13
