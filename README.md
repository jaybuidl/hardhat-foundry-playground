# <h1 align="center"> Hardhat x Foundry Experiment </h1>

![Github Actions](https://github.com/jaybuidl/hardhat-foundry-template/workflows/test/badge.svg)

### Getting Started

 * Use Foundry: 
```bash
forge install
forge test
```

 * Use Hardhat:
```bash
yarn install
yarn test
```

### Features

 * Write / run tests with either Hardhat or Foundry:
```bash
forge test
# or
yarn test
```

 * Use Hardhat's task framework
```bash
yarn hardhat example
```

 * Install libraries with Hardhat.
```bash
yarn add @openzeppelin/contracts
```

 * Install libraries with Foundry which work with Hardhat.
```bash
forge install rari-capital/solmate # Already in this repo, just an example
```

### Notes

Whenever you install new libraries using Foundry, make sure to update your `remappings.txt` file by running `forge remappings > remappings.txt`. This is required because we use `hardhat-preprocessor` and the `remappings.txt` file to allow Hardhat to resolve libraries you install with Foundry.
