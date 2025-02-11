# GateChain Account Types

GateChain offers multiple account types to meet different security requirements. This article will introduce the various account types and their characteristics.

## Account Types Overview

GateChain supports the following account types:

| Account Type | Prefix | Key Features | Use Cases |
|-------------|---------|--------------|-----------|
| Normal Account | gt | - Single private key control<br>- Immediate transactions<br>- Basic functionality | Daily transactions and transfers |
| Vault Account | vault | - Delayed transactions<br>- Clearing period<br>- Recovery account support | Large asset storage and enhanced security |
| Multi-signature Account | gt1m | - Multiple signature requirement<br>- Configurable threshold<br>- Shared control | Team funds and organizational assets |
| EVM Account | 0x | - Ethereum compatible<br>- Smart contract interaction<br>- Web3 wallet support | DApp interaction and smart contract deployment |

### 1. Normal Account

Normal accounts are the basic account type with the following features:

- Controlled by a single private key
- Transactions take effect immediately
- Suitable for daily transfers and transactions
- Account prefix is "gt"

### 2. Vault Account

Vault accounts are GateChain's unique secure account type with the following features:

- Supports delayed transactions
- Has clearing period
- Configurable recovery account
- Account prefix is "vault"

Main parameters for vault accounts:

| Parameter | Description |
|------|------|
| delay_height | Transaction delay effective height |
| clearing_height | Account clearing height |
| security_address | Recovery account address |


### 3. Multi-signature Account

Multi-signature accounts require multiple private keys to sign transactions, with these features:

- Requires multiple account signatures
- Can set signature threshold
- Suitable for team or organization use
- Provides higher security

## Account Address Format

GateChain account addresses consist of:

- Account type prefix
- Base58 encoded public key hash
- Checksum

Examples:
- Normal account: gt1p0xl8jqr...
- Vault account: vault1p0xl8jq...
- Multi-sig account: gt1m0xl8jqr...

## EVM Account

EVM accounts are fully compatible with Ethereum Virtual Machine, offering the following features:

- Standard Ethereum address format (0x prefix)
- Compatible with Ethereum tools and wallets (MetaMask, etc.)
- Supports ERC20, ERC721, and other Ethereum standards
- Can interact with GateChain's EVM-compatible smart contracts
- Seamless integration with Web3 applications

EVM accounts enable users to:
- Deploy and interact with smart contracts
- Participate in DeFi protocols
- Use existing Ethereum development tools
- Transfer tokens between GateChain and other EVM chains

## Best Practices

1. Choose appropriate account type based on security needs
2. Use vault accounts for storing large assets
3. Use multi-sig accounts for team fund management
4. Safely store private keys and mnemonic phrases
5. Regularly check account security settings
