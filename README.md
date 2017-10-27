Bch BIP39 Mnemonics
=======

[![NPM Package](https://img.shields.io/npm/v/bch-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/bch-mnemonic)
[![Build Status](https://img.shields.io/travis/owstack/bch-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/owstack/bch-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/owstack/bch-mnemonic.svg?style=flat-square)](https://coveralls.io/r/owstack/bch-mnemonic)

A module for [bch](https://github.com/owstack/bch) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bch-mnemonic
bower install bch-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bch.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('@owstack/bch-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/owstack/bch/blob/master/CONTRIBUTING.md) on the main bch repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/owstack/bch/blob/master/LICENSE).

Copyright 2017 Open Wallet Stack.
