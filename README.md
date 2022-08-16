# Simple Cards

So here,
* We will build a game contract where there is a pack of cards.
* Each card has a number associated with it which ranges from 0 to 2²⁵⁶–1
* Player will guess a number that is going to be picked up.
* The dealer will then at random pick up a card from the pack
* If someone correctly guesses the number, they win 0.1 ETH
* We will hack this game today :)

# How we can prevent this attack

* Don't use blockhash, block.timestamp, or really any sort of on-chain data as sources of randomness.
* You can use oracles like, [Chainlink VRF's](https://docs.chain.link/docs/chainlink-vrf/) for true source of randomness


# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
GAS_REPORT=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```
