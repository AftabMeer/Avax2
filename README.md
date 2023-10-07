# Assessment Contract and Dapp

This repository contains a Solidity smart contract named `Assessment.sol` and a simple React Dapp with an Ethereum integration that interacts with the contract. The contract and Dapp provide basic functionality for managing an Ethereum wallet's balance, including depositing and withdrawing Ether.

## Smart Contract - `Assessment.sol`

### Description
`Assessment.sol` is a Solidity smart contract that allows an owner (presumably the contract deployer) to manage an Ether balance associated with the contract. It provides the following features:

- Constructor: Initializes the contract with an initial balance.
- `getBalance()`: Allows anyone to check the current balance of the contract.
- `deposit(uint256 _amount)`: Allows the owner to deposit Ether into the contract.
- `withdraw(uint256 _withdrawAmount)`: Allows the owner to withdraw Ether from the contract, provided the balance is sufficient.

### Usage
1. Deploy the contract by specifying an initial balance.
2. The owner can deposit and withdraw Ether using the respective functions.
3. Users can check the contract's balance using `getBalance()`.

## React Dapp - `index.js`

### Description
`index.js` is a React-based decentralized application (Dapp) that interacts with the `Assessment` smart contract. It allows users to connect their MetaMask wallet and perform the following actions:

- Connect their MetaMask wallet.
- Check their connected wallet's account address and balance.
- Deposit 1 Ether into the contract.
- Withdraw 1 Ether from the contract.

### Usage
1. Ensure you have MetaMask installed and configured in your browser.
2. Open the Dapp in a browser that supports Ethereum and MetaMask.
3. Click the "Connect your MetaMask wallet" button to connect your wallet.
4. After connecting, you will see your account address and balance.
5. Use the "Deposit 1 ETH" button to deposit 1 Ether into the contract.
6. Use the "Withdraw 1 ETH" button to withdraw 1 Ether from the contract.

## Deployment Script - `deploy.js`

### Description
`deploy.js` is a Hardhat deployment script that deploys the `Assessment` smart contract to the Ethereum blockchain with an initial balance.

### Usage
1. Make sure you have [Hardhat](https://hardhat.org) installed and configured.
2. Execute the script using `npx hardhat run deploy.js` to deploy the `Assessment` contract with an initial balance of 1 Ether.
3. After successful deployment, you will receive the contract's address.

## Prerequisites

- [Hardhat](https://hardhat.org) for smart contract development and deployment.
- [MetaMask](https://metamask.io/) or a compatible Ethereum wallet for interacting with the Dapp.

Make sure you have the necessary dependencies and tools installed before using this code.
