# Status Updates

Get the latest updates from the GateChain team.

## GateChain Mainnet Upgrade v1.1.6

### Overview

1. GateChain consensus version will be upgraded to `v1.1.6`. All nodes participating in the consensus need to upgrade their node binary.

2. Scheduled Upgrade Date: 2024-08-26

3. For detailed information, please refer to the [GateChain Documentation](https://www.gatechain.io/docs/en/developers/gatechain-build/)

### Upgrade Mechanism

The GateChain consensus upgrade process works as follows:

- When a consensus node uses the new binary version for block assembly, it triggers a network-wide upgrade vote
- Once the vote count exceeds the threshold after a round of block creation, the new protocol consensus takes effect network-wide
- At this point, any consensus nodes that haven't upgraded to the latest version will be unable to participate in consensus

### Changelog

1. EVM Version Upgrade

2. Minimum GasPrice Adjustments:
   - Increased from `5NANOGT` to `10NANOGT`
   - Block Gas Limit set to `150M`

3. EIP-2718 Compatibility:
   - Added support for multiple EVM transaction types

4. EIP-1559 Compatibility:
   - Implemented dynamic network fees
   - Introduced base fee burning mechanism

5. RPC Interface Improvements:
   - Process optimization
   - Bug fixes and stability improvements

6. Compilation and UX Enhancements:
   - Added support for local account creation with default password

7. General Improvements:
   - Various bug fixes and optimizations

### Important Notice

Please download and upgrade to the latest version promptly to prevent consensus account disconnection.

---

## GateChain Mainnet Upgrade v1.1.5

### Overview

1. GateChain consensus version will be upgraded to `v1.1.5`. All nodes participating in the consensus need to upgrade their node binary.

2. Scheduled Upgrade Date: 2022-12-20

3. For detailed information, please refer to the [GateChain Documentation](https://www.gatechain.io/docs/en/developers/gatechain-build/)

### Upgrade Mechanism

The GateChain consensus upgrade process works as follows:

- When a consensus node uses the new binary version for block assembly, it triggers a network-wide upgrade vote
- Once the vote count exceeds the threshold after a round of block creation, the new protocol consensus takes effect network-wide
- At this point, any consensus nodes that haven't upgraded to the latest version will be unable to participate in consensus

### Changelog

1. EVM Module Enhancements:
   - Added pledge reward reinvestment function
   - Added one-click reward extraction for all consensus nodes

2. Protocol Compatibility:
   - Compatible with the `EIP-1989` proposal

3. Consensus Improvements:
   - Optimized loyalty coefficient growth plan for committee-selected consensus nodes

4. General Improvements:
   - Various bug fixes and optimizations

### Important Notice

Please download and upgrade to the latest version promptly to prevent consensus account disconnection.

---

## GateChain Mainnet Upgrade v1.1.4

### Overview

1. GateChain consensus version will be upgraded to `v1.1.4`. All nodes participating in the consensus need to upgrade their node binary.

2. Scheduled Upgrade Date: 2022-11-03

3. For detailed information, please refer to the [GateChain Documentation](https://www.gatechain.io/docs/en/developers/gatechain-build/)

### Upgrade Mechanism

The GateChain consensus upgrade process works as follows:

- When a consensus node uses the new binary version for block assembly, it triggers a network-wide upgrade vote
- Once the vote count exceeds the threshold after a round of block creation, the new protocol consensus takes effect network-wide
- At this point, any consensus nodes that haven't upgraded to the latest version will be unable to participate in consensus

### Changelog

1. Node Improvements:
   - Added user-editable fee-rate for consensus nodes
   - Implemented "debug trace" for EVM transactions

2. System Enhancements:
   - Added batch number rollback capability with Gatemint engine

3. General Improvements:
   - Various bug fixes and optimizations

### Important Notice

Please download and upgrade to the latest version promptly to prevent consensus account disconnection.

---

## GateChain Mainnet Upgrade v1.1.3

### Overview

1. GateChain consensus version will be upgraded to `v1.1.3`. All nodes participating in the consensus need to upgrade their node binary.

2. Scheduled Upgrade Date: 2022-05-17

3. For detailed information, please refer to the [GateChain Documentation](https://www.gatechain.io/docs/en/developers/gatechain-build/)

### Upgrade Mechanism

The GateChain consensus upgrade process works as follows:

- When a consensus node uses the new binary version for block assembly, it triggers a network-wide upgrade vote
- Once the vote count exceeds the threshold after a round of block creation, the new protocol consensus takes effect network-wide
- At this point, any consensus nodes that haven't upgraded to the latest version will be unable to participate in consensus

### Changelog

1. System Upgrades:
   - Upgraded consensus version to `v1.1.3`
   - Enhanced Ledger snapshot functionality

2. Performance Improvements:
   - Implemented gas fee recommendations
   - Added transaction sorting by gas price
   - Added signature cache for improved EVM transaction efficiency

3. Module Enhancements:
   - Optimized subscription push module
   - Fixed power update timing in EVM staking

### Important Notice

Please download and upgrade to the latest version promptly to prevent consensus account disconnection.

---

## GateChain Mainnet Upgrade v1.1.0

### Overview

1. GateChain consensus version will be upgraded to `v1.1.0`. All nodes participating in the consensus need to upgrade their node binary.

2. Scheduled Upgrade Date: 2021-09-15

3. For detailed information, please refer to the [GateChain Documentation](https://www.gatechain.io/docs/en/developers/gatechain-build/)

### Upgrade Mechanism

The GateChain consensus upgrade process works as follows:

- When a consensus node uses the new binary version for block assembly, it triggers a network-wide upgrade vote
- Once the vote count exceeds the threshold after a round of block creation, the new protocol consensus takes effect network-wide
- At this point, any consensus nodes that haven't upgraded to the latest version will be unable to participate in consensus

### Changelog

1. Version Upgrades:
   - Upgraded consensus version to `v1.1.0`
   - Upgraded EVM version to `v1.10.8`

2. System Improvements:
   - Implemented caching for transactions with large nonce values
   - Enhanced `API debug_traceTransaction` with failed transaction debugging support

### Important Notice

Please download and upgrade to the latest version promptly to prevent consensus account disconnection.

---

## GateChain Launch Announcement

### Overview

GateChain is a next-generation public blockchain, focused on onchain asset safety and decentralized trading. With a uniquely designed Vault Account, primed for handling abnormal transactions, GateChain presents an extraordinary clearing mechanism, tackling the challenges of asset theft and private key loss. Decentralized trading and cross-chain transfers will also be supported, alongside other core features.