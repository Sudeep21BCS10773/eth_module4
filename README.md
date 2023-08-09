# eth_module4
# DegenGamingToken Contract
This Solidity smart contract implements the DegenGamingToken, an ERC-20 compatible token with additional functionality for a gaming platform. This token can be used for in-game transactions, rewards, and prize redemptions.

# Table of Contents
Overview
Features
Getting Started
Usage
Functions
Events
License

# Overview
The DegenGamingToken contract is an Ethereum smart contract that extends the functionality of ERC-20 tokens. It incorporates the OpenZeppelin contracts for ERC-20 implementation and access control through ownership. This token is designed for use within a gaming ecosystem, enabling users to perform various actions, including minting new tokens, redeeming prize money, checking balances, and burning tokens.

# Features
Minting: The contract owner can mint new tokens to a specified address.
Prize Redemption: Users can redeem prize money if they hold a sufficient balance. The redeemed amount decreases over time.
Balances: Users can check their token balances.
Burning: Users can burn their tokens to reduce their balance.

# Getting Started
Clone or download the repository.
Install the required dependencies:
Deploy the contract on an Ethereum-compatible blockchain.

# Usage
This contract is intended to be deployed on an Ethereum-compatible blockchain. It provides a token that can be used within a gaming platform. To use the token, you'll need to interact with its functions through transactions.

# Functions
mint(address account, uint256 amount): Mints new tokens and assigns them to the specified address. Only the contract owner can call this function.

redeem(): Allows users to redeem their prize money if their balance is sufficient and the prize money is available. The redeemed amount decreases over time. After redemption, in-game redemption logic can be performed.

burn(uint256 amount): Burns (destroys) the specified amount of tokens from the caller's balance.

checkBalance(address account): Returns the token balance of the specified account.

# Events
Redeemed(address indexed user, uint256 redeemedAmount, uint256 newPrizeMoney): Emitted when a user redeems their prize money. Provides information about the user, the redeemed amount, and the remaining prize money.

# License
This project is licensed under the MIT License. You can find a copy of the license in the LICENSE file.
