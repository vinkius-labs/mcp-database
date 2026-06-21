# Ankr (Web3 Node API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ankr-web3-node-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access high-performance Web3 RPC nodes via Ankr. Query block data, check wallet balances, and interact with smart contracts across multiple EVM chains.

## Description
Connect your AI agent to **Ankr's** global node infrastructure and interact with blockchain data through natural language. This server provides a direct bridge to Ethereum and other EVM-compatible chains.

### What you can do

- **Chain Queries** — Fetch the latest block numbers and detailed block information by hash or number across supported networks.
- **Account Auditing** — Check wallet balances, transaction counts (nonces), and retrieve the smart contract code at any address.
- **Transaction Analysis** — Inspect transaction details and receipts, or estimate gas costs for potential on-chain operations.
- **Smart Contract Interaction** — Execute `eth_call` to read contract states or simulate complex multi-transaction scenarios with `eth_simulateV1`.
- **State Inspection** — Access raw storage slots with `eth_getStorageAt` and filter event logs with `eth_getLogs` for deep data analysis.

### How it works

1. Subscribe to this server
2. Enter your Ankr JWT Token
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

No more manual JSON-RPC requests or complex Postman setups. Your AI acts as a blockchain developer or data analyst.

### Who is this for?

- **Web3 Developers** — quickly debug smart contracts, check nonces, and verify deployments directly from the IDE.
- **DeFi Researchers** — analyze on-chain state, simulate transactions, and fetch historical logs without writing custom scripts.
- **Data Analysts** — retrieve real-time blockchain metrics and block data for reporting and monitoring.


## Available Tools
- **ankr_getAccountBalance**: Retrieves all token balances for a wallet
- **ankr_getBlocks**: Retrieves full info for a range of blocks
- **ankr_getInteractions**: Lists all blockchains a wallet has interacted with
- **ankr_getNFTHolders**: Lists all holders of a specific NFT collection
- **ankr_getNFTMetadata**: Retrieves metadata for a specific NFT
- **ankr_getNFTsByOwner**: Retrieves all NFTs owned by an address across multiple chains
- **ankr_getTokenPrice**: Returns the current USD price of a token
- **ankr_getTokenTransfers**: Returns historical token transfer data
- **eth_blockNumber**: Returns the most recent block number
- **eth_call**: Executes a call without creating a transaction
- **eth_estimateGas**: Estimates gas needed for a transaction
- **eth_getBalance**: Returns the balance of an address
- **eth_getBlockByHash**: Returns block information by hash
- **eth_getBlockByNumber**: Returns block information by number
- **eth_getCode**: Returns the code at a given address
- **eth_getLogs**: Returns logs matching filter criteria
- **eth_getStorageAt**: Returns the value from a storage position
- **eth_getTransactionByHash**: Returns transaction details
- **eth_getTransactionCount**: Returns the number of transactions sent from an address (nonce)
- **eth_getTransactionReceipt**: Returns the receipt of a transaction
- **eth_sendRawTransaction**: Submits a signed transaction to the network
- **eth_simulateV1**: Simulates multiple blocks/transactions
- **getAccountInfo**: Returns all info associated with a Pubkey
- **getBalance**: Returns the lamport balance of an account
- **getBlockHeight**: Returns the current block height
- **getBlock**: Returns identity and transaction info for a confirmed block
- **getEpochInfo**: Returns information about the current epoch
- **getLatestBlockhash**: Returns the latest blockhash for transaction building
- **getProgramAccounts**: Returns all accounts owned by a program
- **getTransaction**: Returns details for a confirmed transaction
- **sendTransaction**: Submits a signed transaction
- **simulateTransaction**: Simulates a transaction to check for errors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ankr (Web3 Node API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest block number on Ethereum?"

**🤖 AI Agent:**
> I've checked the Ethereum network. The most recent block number is 19,245,812.

---

**👤 You:**
> "Check the balance of address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e on the 'eth' chain."

**🤖 AI Agent:**
> The balance for that address on Ethereum is 1,500,000,000,000,000,000 Wei (1.5 ETH).

---

**👤 You:**
> "Get the transaction receipt for hash 0x5c504ed432cb511db3b32169e5444570f9d0cad662f6e19df34ad57d57ad5 on eth."

**🤖 AI Agent:**
> I've retrieved the receipt. The transaction was successful, included in block 18,450,210, and used 21,000 gas.


## ❓ FAQ

**Q: How can I check the current block height on a specific network?**
Use the `eth_blockNumber` tool and provide the `chain_alias` (e.g., 'eth' for Ethereum). The agent will return the most recent block number recorded on that chain.

**Q: Is it possible to simulate a transaction before sending it to the mainnet?**
Yes! You can use the `eth_simulateV1` tool. By providing a simulation payload, you can see the potential outcome and state changes of transactions without actually broadcasting them.

**Q: How do I retrieve the balance of a specific wallet address?**
Simply use the `eth_getBalance` tool with the target `address` and `chain_alias`. The agent will fetch the current balance in Wei for that account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ankr-web3-node-api](https://vinkius.com/mcp/ankr-web3-node-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ankr (Web3 Node API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ankr-web3-node-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ankr (Web3 Node API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ankr-web3-node-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
