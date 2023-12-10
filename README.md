# DEGEN Token Smart Contract 

## Overview

The DEGEN Token smart contract is a decentralized application (DApp) developed on the Ethereum blockchain. It implements the ERC-20 token standard, allowing users to create, transfer, and redeem DEGEN tokens. Additionally, it incorporates the Ownable contract from OpenZeppelin, enabling ownership management functionalities.

## Features

- ERC-20 Compliance: DEGEN Token adheres to the ERC-20 standard, providing compatibility with various decentralized applications and exchanges.
- Minting: The contract owner can mint new DEGEN tokens.
- Burning: Token holders can burn their tokens, reducing the total supply.
- Transferring Tokens: Users can transfer DEGEN tokens to other addresses.
- Sneaker Redemption: Users can redeem limited edition sneakers by exchanging tokens.

## Usage

### Minting

The contract owner can mint new DEGEN tokens by calling the `mint` function, specifying the recipient's address and the amount of tokens to mint.

### Burning

Token holders can burn their tokens by calling the `burn` function, specifying the total amount of tokens to burn.

### Transferring Tokens

Users can transfer DEGEN tokens to other addresses using the `transferTokens` function.

### Redeeming Sneakers

Users can redeem limited edition sneakers by calling the `redeemSneaker` function, providing the index of the desired sneaker.

## Contract Structure

### DEGENToken

The main contract inheriting from ERC-20 and Ownable, implementing token-related functionalities.

### Events

- `Minted`: Triggered when new tokens are minted.
- `Transferred`: Triggered when tokens are transferred between addresses.
- `Redeemed`: Triggered when a user redeems a limited edition sneaker.

### Structs

- `Sneaker`: Defines the structure of limited edition sneakers, including a unique tokenId and the number of tokens required for redemption.

## Security Considerations

- The contract owner has special privileges, so ownership should be transferred to a multisig wallet for enhanced security.
- Ensure that proper testing is conducted before deploying the contract to the Ethereum mainnet.
- Be cautious when interacting with contracts to avoid potential vulnerabilities.

## License

This smart contract is released under the MIT License. See the [LICENSE](./LICENSE) file for details.

