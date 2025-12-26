# Celestial Rift (Built for Base)

Celestial Rift is a streamlined, read-only onchain tool crafted for Base Mainnet and Base Sepolia. This tool offers developers the ability to verify network authenticity, examine blockchain data, and interact with deployed contracts via Coinbase Wallet SDK, while also validating the results with independent verification through Basescan.

---

## Key Features

- **Coinbase Wallet SDK Integration** for easy connection via EIP-1193  
- **Base ChainId Verification** for both Mainnet (8453) and Sepolia (84532)  
- **Network Snapshotting** to capture block details, gas price, and gas usage  
- **Address Inspection** to retrieve balances, transaction history, and check bytecode  
- **ERC-20 Token Analysis** to view metadata, total supply, and balance for specific tokens  
- **Basescan Validation** to cross-check addresses and contracts for accuracy  

---

## Project Structure

- **app/celestial-rift.ts**  
  The main script that connects to Coinbase Wallet and queries Base’s RPC endpoints for real-time blockchain data.

- **config/base.networks.json**  
  Contains configuration information for Base networks, including RPC URLs, chainIds, and explorer URLs for Base Mainnet and Sepolia.

- **scripts/sample-addresses.json**  
  A collection of sample addresses for consistent and repeatable testing.

- **contracts/**  
  Solidity contracts deployed to Base Sepolia for testing purposes:
  - `structs.sol` — contract demonstrates the use of structs in Solidity
  - `inheritance.sol` — allows a contract (child) to inherit functionality from another contract (parent)

- **package.json**  
  Lists the project's dependencies, including necessary SDKs and references to Base and Coinbase repositories.

- **README.md**  
  The document you are currently reading, which explains how to use and understand the project.

---

## Supported Networks

- **Base Sepolia**  
  ChainId (decimal): 84532  
  Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

- **Base Mainnet**  
  ChainId (decimal): 8453  
  Explorer: [basescan.org](https://basescan.org)

---

## Functionality

Celestial Rift is a robust tool that allows developers to:
- Connect to **Coinbase Wallet SDK** for secure wallet access
- Interact with **Base RPC** to query network data in real-time
- Inspect blockchain states, blocks, and gas metrics  
- Perform read-only operations such as inspecting addresses and contract metadata  
- Cross-check results using **Basescan** to verify accuracy  

Everything in Celestial Rift is non-invasive and read-only, ensuring no transactions are broadcast to the network.

---

## Dependencies

This project integrates the following open-source tools:
- **Coinbase Wallet SDK** for secure wallet connections  
- **OnchainKit** for seamless interaction with Base-native primitives  
- **Viem** for efficient, type-safe RPC communication  
- Direct dependencies from **Base** and **Coinbase** repositories  

---

## License

MIT License

Copyright (c) 2025 YOUR_NAME

---

## Author Information

GitHub: [https://github.com/owing-evident](https://github.com/owing-evident)  

Email: owing.evident.0p@icloud.com 

X profile: [https://x.com/thortus1847](https://x.com/thortus1847)  

---

## Testnet Deployment on Base Sepolia

To confirm the functionality of the tools and validate network interactions, the following contracts have been deployed to the Base Sepolia test network:

**Network**: Base Sepolia  
**ChainId (decimal)**: 84532  
**Explorer**: [sepolia.basescan.org](https://sepolia.basescan.org)

**Contract structs.sol address**:  
0xe7dc3993Af86af69fBBBc08d1d87Ec93115f9069

Deployment and verification:
- [Deployment link](https://sepolia.basescan.org/address/0xe7dc3993Af86af69fBBBc08d1d87Ec93115f9069)
- [Code verification](https://sepolia.basescan.org/0xe7dc3993Af86af69fBBBc08d1d87Ec93115f9069/0#code)

**Contract inheritance.sol address**:  
0x5443b9565c6b1C853BCfB8921C7d684F463203C3

Deployment and verification:
- [Deployment link](https://sepolia.basescan.org/address/0x5443b9565c6b1C853BCfB8921C7d684F463203C3)
- [Code verification](https://sepolia.basescan.org/0x5443b9565c6b1C853BCfB8921C7d684F463203C3/0#code)

These deployments help confirm that Base tooling and network interactions are functioning as expected prior to launching on Mainnet.
