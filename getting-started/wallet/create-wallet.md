# Create GateChain Wallet

This guide will show you how to create and manage a GateChain wallet.

## Creation Methods

GateChain offers multiple ways to create a wallet:

1. Command Line Tool
2. Web Wallet
3. SDK Integration

## Command Line Creation

### 1. Install CLI Tool

```bash
# Download the latest version
git clone https://github.com/gatechain/gatechain-cli
cd gatechain-cli

# Install dependencies
make install
```

### 2. Create New Wallet

```bash
gatechain-cli keys add <wallet-name>
```

The system will generate:
- Wallet address
- Private key
- Mnemonic phrase (please store securely)

### 3. Import Existing Wallet

```bash
# Import via mnemonic phrase
gatechain-cli keys add <wallet-name> --recover

# Import via private key
gatechain-cli keys add <wallet-name> --private-key <private-key>
```

## Using Web Wallet

### 1. Access Official Wallet

Visit [GateChain Web Wallet](https://www.gatechain.io/wallet)

### 2. Create Wallet

1. Click "Create Wallet"
2. Set wallet password
3. Backup mnemonic phrase
4. Verify mnemonic phrase
5. Complete creation

### 3. Import Wallet

1. Click "Import Wallet"
2. Choose import method:
   - Mnemonic phrase import
   - Private key import
   - Keystore import
3. Enter required information
4. Set wallet password
5. Complete import

## SDK Integration

### JavaScript SDK

```javascript
const { GateChain } = require('gatechain-sdk');

// Create wallet
const wallet = GateChain.createWallet();

// Get address
console.log(wallet.address);

// Get private key
console.log(wallet.privateKey);

// Get mnemonic phrase
console.log(wallet.mnemonic);
```

### Python SDK

```python
from gatechain import Wallet

# Create wallet
wallet = Wallet.create()

# Get address
print(wallet.address)

# Get private key
print(wallet.private_key)

# Get mnemonic phrase
print(wallet.mnemonic)
```

## Security Recommendations

1. Backup Management
   - Securely backup mnemonic phrase
   - Multiple backups of private key
   - Encrypted storage of Keystore

2. Usage Recommendations
   - Use hardware wallet
   - Enable multi-signature
   - Regular password updates

3. Important Notes
   - Never share private keys
   - Beware of phishing websites
   - Regular data backups
   - Careful with authorizations

## Common Issues

1. Forgot Password?
   - Recover using mnemonic phrase
   - Re-import using private key

2. Cannot Import Address?
   - Check address format
   - Verify network connection
   - Update wallet version

3. Assets Not Showing?
   - Confirm network connection
   - Check token contract
   - Refresh wallet page
