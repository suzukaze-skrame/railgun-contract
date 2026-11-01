# RAILGUN Contracts

## Getting started

- Install Node.js - using [nvm](https://github.com/nvm-sh/nvm) is recommended
- Run `npm i` to install dependencies
- (Optional) Setup hardhat local network config in `~/.hardhat/networks.{js|ts|json}` following the [hardhat-local-networks-config-plugin](https://github.com/facuspagnuolo/hardhat-local-networks-config-plugin) format.
- (Optional) Install `hardhat-shorthand` to use `hh` commands.
- Run `hh help` or `npx hardhat help` for list of commands

## Local deployment

[Getting started with the contracts](https://docs.railgun.org/developer-guide/engine-1/getting-started-with-the-contracts)

```bash
# 1. Install dependencies
npm install

# 2. Start a local chain (choose one)
npx hardhat node  # Hardhat
anvil             # Anvil (requires Foundry)

# 3. Deploy in another terminal
npx hardhat deploy:test --network localhost
```

Use the `proxy` address printed in `DEPLOY CONFIG` as the RAILGUN core wallet address in your client. As described in the official guide above, `proxy` is the upgradeable entry point for the `implementation` contract.
