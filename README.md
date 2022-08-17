# discarbon-devcon-attendee-contract
This the smart contract for the devcon attendees to buy carbon tokens and send them to a wallet.

This smart contract has the following tasks:

1. Receive/Get coins/tokens from attendee.
2. Exchange for carbon token (NCT) on sushiswap.
3. Forward carbon token to a preprogrammed wallet address.
4. Store the attendee address and offset amount to issue a POAP.


## How to get started

Install all dependencies

```npm install```

copy the "env" file to ".env" and fill in the needed Keys.

Fork the polygon mainnet

```hh node```

(need to have hardhat shorthand installed for this: ```npm i -g hardhat-shorthand```)

Deploy the pooling contract with:

`hh run scripts/deploy.js`


## Tests

Run tests using:

`hh test`

You can also run a forked chain locally and then deploy test on it by running:

`hh node`

in the first terminal window and:

`hh test --network localhost`

in the second terminal window to run the tests.

You can also locally deploy the contracts manually using:

`hh run scripts/deploy.js --network localhost`

## hardhat sample project readme

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
GAS_REPORT=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```
