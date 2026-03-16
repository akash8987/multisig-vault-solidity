# Multi-Sig Vault

A secure, expert-level Multi-Signature Wallet implementation for Ethereum-based blockchains. This repository provides a flat-file structure for a robust "M-of-N" wallet where a defined number of owners must confirm a transaction before it can be executed.

### Features
* **M-of-N Authorization**: Set custom thresholds for transaction approval.
* **Gas Efficiency**: Optimized storage patterns to reduce transaction costs.
* **Security First**: Prevents re-entrancy and protects against unauthorized access.
* **Event Logging**: Full traceability for submissions, confirmations, and executions.

### How to Use
1. Deploy `MultiSigVault.sol` with an array of owner addresses and the required number of confirmations.
2. Use `submitTransaction` to propose a transfer.
3. Other owners call `confirmTransaction`.
4. Once the threshold is met, anyone can call `executeTransaction`.
