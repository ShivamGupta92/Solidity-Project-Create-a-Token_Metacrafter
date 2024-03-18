# Solidity-Project-Create-a-Token_Metacrafter


## Table of Contents

- [MyETHToken](#myethtoken)
- [Specifications](#specifications)
- [Instructions](#instructions)

## MyETHToken

This is a basic ERC-20 token contract developed in Solidity. The contract facilitates token creation, destruction, and storage of token-related information.

## Specifications

The contract includes public variables to hold details about the token:

- tokenName: A string indicating the token's name.
- abbrv: A string representing the token's abbreviation.
- totalSupply: An unsigned integer indicating the total token supply.

Additionally, the contract features a mapping of addresses to token balances:

- balances: A mapping linking addresses to their corresponding token balances.

The contract incorporates a mint function to increase the total supply and the balance of a designated address by a specified value:

Parameters:
- _address: The address where the tokens will be minted.
- _value: The quantity of tokens to be minted.

Actions:
- Increment the totalSupply by _value.
- Increase the balance of _address by _value.

Moreover, a burn function is included to decrease the total supply and the balance of a designated address by a specified value:

Parameters:
- _address: The address from which tokens will be burned.
- _value: The quantity of tokens to be burned.

Actions:
- Validate if the balance of _address is greater than or equal to _value.
- If true, decrease the totalSupply by _value.
- Decrease the balance of _address by _value.

## Instructions

Deploy the MyETHToken contract on a compatible Ethereum network.

Once deployed, interact with the contract by invoking the following functions:

- mint: Generates new tokens and allocates them to a specified address.

Parameters:
- _address: The address to which tokens will be minted.
- _value: The quantity of tokens to be minted.

- burn: Eliminates existing tokens by reducing the total supply and the balance of a specified address.

Parameters:
- _address: The address from which tokens will be burned.
- _value: The quantity of tokens to be burned.

## Author
- Shivam
