# GateChain Account Types

GateChain offers multiple account types to meet different security requirements. This article will introduce the various account types and their characteristics.

## Account Types Overview

GateChain supports the following account types:

1. Normal Account
2. Vault Account
3. Multi-signature Account

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

#### Create Vault Account

Create vault account via API:

```bash
POST /v1/vault-account/create/{base-account}
```

#### Modify Clearing Height

```bash
POST /v1/vault-account/update-clearing-height
```

#### Account Clearing

```bash
POST /v1/vault-account/clear
```

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

## Best Practices

1. Choose appropriate account type based on security needs
2. Use vault accounts for storing large assets
3. Use multi-sig accounts for team fund management
4. Safely store private keys and mnemonic phrases
5. Regularly check account security settings
