# Aleo Wallet Adapters

## Description

`aleo-wallet-adapters` is a library that provides adapters for multiple Aleo wallets, enabling seamless integration and interaction with different Aleo wallets in your application. Currently, it supports Leo Wallet, Soter Wallet, Fox Wallet, and Puzzle Wallet.

## Installation

To install the package, run the following command in your project directory:

```bash
npm install aleo-wallet-adapters
```

## Usage

The usage of `aleo-wallet-adapters` is similar to that of the Leo wallet adapter. You can initialize the adapters for supported wallets and use them in your application. Here's an example of how to use the adapters in a React application:

```javascript
import React, { useMemo } from 'react';
import {
  LeoWalletAdapter,
  SoterWalletAdapter,
  FoxWalletAdapter,
  PuzzleWalletAdapter
} from 'aleo-wallet-adapters';

const MyComponent = () => {
  const wallets = useMemo(() => [
    new LeoWalletAdapter({
      appName: 'Aleo Name Service',
    }),
    new FoxWalletAdapter({
      appName: 'Aleo Name Service',
    }),
    new PuzzleWalletAdapter({
      appName: 'Aleo Name Service',
    }),
    new SoterWalletAdapter({
      appName: 'Aleo Name Service',
    })
  ], []);

  // Your component logic here

  return (
    <div>
      {/* Your component UI here */}
    </div>
  );
};

export default MyComponent;
```

## Supported Wallets
* **Leo Wallet**: An Aleo wallet adapter for Leo Wallet.
* **Fox Wallet**: An Aleo wallet adapter for Fox Wallet.
* **Puzzle Wallet**: An Aleo wallet adapter for Puzzle Wallet.
* **Soter Wallet**: An Aleo wallet adapter for Soter Wallet.


## Contributing
Contributions to `aleo-wallet-adapters` are welcome. If you wish to contribute, please submit a pull request or open an issue for discussion.