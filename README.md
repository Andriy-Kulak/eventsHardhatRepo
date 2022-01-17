# Hardhat-Events-Logs

This project demonstrates how to work with events in hardhat. In the `deploy_and_store` script, you'll see the output of the events. 

 ## Requirements

- [nodejs](https://nodejs.org/en/download/)
  - You can test it's installed by running `node --version`
- [yarn](https://yarnpkg.com/)
  - You can test it's installed by running `yarn --version`
- [git](https://git-scm.com/downloads)
  - You can test it's installed by running `git --version`

## Installation

Clone this repo & install dependencies
```sh
git clone https://github.com/PatrickAlphaC/hardhat-events-logs
cd hardhat-events-logs
yarn
```

## Quickstart

Run:
```
npx hardhat run scripts/deploy_and_store.js
```

This will print out the events from our smart contracts. 

Then, create a `.env` file and add the following lines:
```
ETHERSCAN_API_KEY=ABC123ABC123ABC123ABC123ABC123ABC1
RINKEBY_RPC_URL=https://eth-ropsten.alchemyapi.io/v2/<YOUR ALCHEMY KEY>
PRIVATE_KEY=YOUR_BLOCKCHAIN_WALLET_PRIVATE_KEY
```
DO NOT PUSH YOUR PRIVATE_KEY TO GITHUB. Please test and develop with a private key that doesn't have any real money in it. 

Follow the [basics tutorial](https://docs.chain.link/docs/beginners-tutorial/) to learn how to get everything setup. 

Then, run:

```sh
hh run scripts/deploy_and_store.js --network rinkeby
```

## Testing

```sh
npx hardhat test
```

## Etherscan verification

Once you've deployed your code, to verify it run:

```shell
npx hardhat verify --network kovan DEPLOYED_CONTRACT_ADDRESS 
```
