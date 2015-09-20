Bitcore
=======

[![NPM Package](https://img.shields.io/npm/v/coinforge.svg?style=flat-square)](https://www.npmjs.org/package/coinforge)
[![Build Status](https://img.shields.io/travis/bitpay/coinforge.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge)
[![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge)


A pure and powerful JavaScript Bitcoin library.

## Principles

Bitcoin is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the Bitcoin network allows for highly resilient bitcoin infrastructure, and the developer community needs reliable, open-source tools to implement bitcoin apps and services.

## Get Started

```
npm install coinforge
```

Using it in Node.js:

```javascript
var coinforge = require('coinforge');

assert(coinforge.Address.isValid('126vMmY1fyznpZiFTTnty3cm1Rw8wuheev'));
var simpleTx = new coinforge.Transaction();
var simpleTx.from(unspent).to(address, amount);
simpleTx.sign(privateKey);
```

## Documentation

The complete docs are hosted here: [coinforge documentation](http://coinforge.io/guide/). There's also a [coinforge API reference](http://coinforge.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each coinforge utility.

- [Read the Developer Guide](http://coinforge.io/guide/)
- [Read the API Reference](http://coinforge.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/coinforge).

## Examples

* [Generate a random address](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#generate-a-random-address)
* [Generate a address from a SHA256 hash](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#create-a-transaction)
* [Sign a Bitcoin message](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#sign-a-bitcoin-message)
* [Verify a Bitcoin message](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](https://github.com/bitpay/coinforge/blob/master/docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)


## Modules
This module provides bitcoin's core features. Other features and protocol extensions are built into separate modules. Here is a list of official coinforge modules:

Module | Version | Building | Coverage
-------|---------|----------|---------
<a href="http://github.com/bitpay/coinforge-payment-protocol"><img src="http://coinforge.io/css/images/coinforge-payment-protocol.svg" alt="coinforge-payment-protocol" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-payment-protocol.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-payment-protocol) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-payment-protocol.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-payment-protocol) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-payment-protocol.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-payment-protocol)
<a href="http://github.com/bitpay/coinforge-p2p"><img src="http://coinforge.io/css/images/coinforge-p2p.svg" alt="coinforge-p2p" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-p2p.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-p2p) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-p2p.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-p2p) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-p2p.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-p2p?branch=master)
<a href="http://github.com/bitpay/coinforge-mnemonic"><img src="http://coinforge.io/css/images/coinforge-mnemonic.svg" alt="coinforge-mnemonic" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-mnemonic) |  [![Build Status](https://img.shields.io/travis/bitpay/coinforge-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-mnemonic) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-mnemonic.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-mnemonic)
<a href="http://github.com/bitpay/coinforge-ecies"><img src="http://coinforge.io/css/images/coinforge-ecies.svg" alt="coinforge-ecies" height="25"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-ecies.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-ecies) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-ecies.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-ecies) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-ecies.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-ecies)
<a href="http://github.com/bitpay/coinforge-channel"><img src="http://coinforge.io/css/images/coinforge-channel.svg" alt="coinforge-channel" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-channel.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-channel) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-channel.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-channel) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-channel.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-channel)
<a href="http://github.com/bitpay/coinforge-explorers"><img src="http://coinforge.io/css/images/coinforge-explorers.svg" alt="coinforge-explorers" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-explorers.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-explorers) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-explorers.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-explorers) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-explorers.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-explorers)
<a href="http://github.com/bitpay/coinforge-message"><img src="http://coinforge.io/css/images/coinforge-message.svg" alt="coinforge-message" height="28"></a> | [![NPM Package](https://img.shields.io/npm/v/coinforge-message.svg?style=flat-square)](https://www.npmjs.org/package/coinforge-message) | [![Build Status](https://img.shields.io/travis/bitpay/coinforge-message.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/coinforge-message) | [![Coverage Status](https://img.shields.io/coveralls/bitpay/coinforge-message.svg?style=flat-square)](https://coveralls.io/r/bitpay/coinforge-message)

## Security

We're using Bitcore in production, as are [many others](http://coinforge.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/bitpay/coinforge/blob/master/CONTRIBUTING.md) file. 

## Building the Browser Bundle

To build coinforge full bundle for the browser:

```sh
gulp browser
```

This will generate files named `coinforge.js` and `coinforge.min.js`.

You can also use our pre-generated files, provided for each release along with a PGP signature by one of the project's maintainers. To get them, checkout a release commit (for example, https://github.com/bitpay/coinforge/commit/e33b6e3ba6a1e5830a079e02d949fce69ea33546 for v0.12.6).

To verify signatures, use the following PGP keys:
- @braydonf: https://pgp.mit.edu/pks/lookup?op=get&search=0x9BBF07CAC07A276D
- @pnagurny: https://pgp.mit.edu/pks/lookup?op=get&search=0x0909B33F0AA53013

## Development & Tests

```sh
git clone https://github.com/bitpay/coinforge
cd coinforge
npm install
```

Run all the tests:

```sh
gulp test
```

You can also run just the Node.js tests with `gulp test:node`, just the browser tests with `gulp test:browser`
or create a test coverage report (you can open `coverage/lcov-report/index.html` to visualize it) with `gulp coverage`.

## License

Code released under [the MIT license](https://github.com/coinforge/coinforge/blob/master/LICENSE).

Copyright 2015 Coinforge Developers.
