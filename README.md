# Metacrafters-Eth-Proof-Beginner
# MyToken

MyToken is a Solidity smart contract that represents a custom token on the Ethereum blockchain. This contract allows you to mint and burn tokens, as well as keep track of token balances for different addresses.

## Overview

The MyToken contract provides the following features:

- Public variables to store the details about the token, including the token name, token abbreviation, and total supply.
- A mapping that associates addresses with their respective token balances.
- A `mint` function that increases the total supply and the balance of a specified address.
- A `burn` function that decreases the total supply and the balance of a specified address.
- The `burn` function includes conditionals to ensure the balance of the address is sufficient for the amount to be burned.

## Getting Started

To use the MyToken contract, follow these steps:

1. Deploy the contract on the Ethereum blockchain using a tool like Remix, an online Solidity IDE.
2. Set the token details by providing the token name, token abbreviation, and total supply during contract deployment.
3. Interact with the contract by calling the `mint` and `burn` functions with appropriate parameters.

## Code Walkthrough

The MyToken contract code is organized as follows:

1. The contract is defined using the `contract` keyword, followed by the contract name (`MyToken`).
2. Public variables `tokenName`, `tokenAbbrv`, and `totalSupply` are declared to store the details about the token.
3. A mapping `balances` is defined to associate addresses with their respective token balances.
4. The constructor is defined to set the token details during contract deployment.
5. The `mint` function takes an address and a value as parameters, increasing the total supply and the balance of the specified address.
6. The `burn` function takes an address and a value as parameters, decreasing the total supply and the balance of the specified address. It includes conditionals to ensure the balance is sufficient for the amount to be burned.

## Usage

1. Deploy the MyToken contract to a supported Ethereum network.

2. Once deployed, you can interact with the contract by calling the following functions:

  mint: Creates new tokens and assigns them to a specified address.

    Parameters:
      _address: The address to which the tokens will be minted.
      _value: The amount of tokens to be minted.
  burn: Destroys existing tokens by reducing the total supply and the balance of a specified address.

    Parameters:
      _address: The address from which the tokens will be burned.
      _value: The amount of tokens to be burned.


## License

This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.
