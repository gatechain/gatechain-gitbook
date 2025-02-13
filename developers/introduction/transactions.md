# Transactions

A transaction is a fundamental concept in blockchain that represents a signed data package, which triggers state changes in the blockchain. Transactions are the only way to modify the state of the blockchain and execute smart contracts.

## Overview

Transactions in blockchain have the following characteristics:
- They are signed messages originated from externally owned accounts (EOA)
- They are transmitted through the network
- They are recorded on the blockchain
- They are the primary mechanism for state changes
- They are required for smart contract execution

## Transaction Structure

A transaction contains the following essential components:

### Basic Fields

| Field | Description |
|-------|-------------|
| Nonce | A sequence number issued by the originating EOA to prevent message replay |
| Gas Price | The price of gas (in wei) the originator is willing to pay |
| Gas Limit | The maximum amount of gas the originator is willing to buy for this transaction |
| Recipient | The destination address |
| Value | The amount of tokens to send to the destination |
| Data | The variable-length binary data payload |

### Signature Components

The transaction includes ECDSA digital signature components:
- v: Signature component for recovery
- r: First 32 bytes of the signature
- s: Second 32 bytes of the signature

### Additional Information

While not part of the actual transaction data structure, the following information can be derived:
- **From Address**: Derived from the ECDSA signature components (v,r,s)
- **Transaction Hash**: Calculated from the transaction data
- **Block Number**: Added once the transaction is mined
- **Timestamp**: The time when the transaction was mined

## Transaction Serialization

Transactions are serialized using the Recursive Length Prefix (RLP) encoding scheme. Key points about serialization:
- All numbers are encoded as big-endian integers
- Field lengths are multiples of 8 bits
- The actual transaction does not contain field labels
- RLP's length prefix is used to identify field boundaries

![Transaction Structure](../../.gitbook/assets/images/transaction.png)

## Important Notes

1. The transaction structure shown above represents the network-serialized format
2. Different clients and applications may store additional metadata
3. The "from" address is derived from the signature components
4. Transaction IDs and block numbers are added after mining