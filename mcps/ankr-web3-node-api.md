# Ankr (Web3 Node API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ankr-web3-node-api)
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


## Available Tools (32)
- **eth_getTransactionByHash**: Use this to check transaction status.

Returns transaction details
- **eth_simulateV1**: Provide a payload detailing the simulation scope.

Simulates multiple blocks/transactions
- **ankr_getAccountBalance**: Supply the chain alias and wallet address.

Retrieves all token balances for a wallet
- **ankr_getBlocks**: Supply the chain alias and the block range object.

Retrieves full info for a range of blocks
- **ankr_getInteractions**: Supply the chain alias and the wallet address.

Lists all blockchains a wallet has interacted with
- **ankr_getNFTHolders**: Supply the chain alias and collection identifier.

Lists all holders of a specific NFT collection
- **ankr_getNFTMetadata**: Provide the chain alias and contract address.

Retrieves metadata for a specific NFT
- **ankr_getNFTsByOwner**: Provide the chain alias and wallet address.

Retrieves all NFTs owned by an address across multiple chains
- **ankr_getTokenPrice**: Provide the chain alias and token identifier.

Returns the current USD price of a token
- **eth_estimateGas**: Use this to prevent transaction failures due to insufficient gas.

Estimates gas needed for a transaction
- **eth_getCode**: Use this to verify contract deployment.

Returns the code at a given address
- **eth_getLogs**: Provide the required filter_criteria object.

Returns logs matching filter criteria
- **eth_getTransactionReceipt**: Use this to confirm execution results.

Returns the receipt of a transaction
- **eth_sendRawTransaction**: Ensure the transaction is correctly signed before calling this tool.

Submits a signed transaction to the network
- **getAccountInfo**: Supply the Pubkey for the target account.

Returns all info associated with a Pubkey
- **getBlock**: Specify the chain alias and block number.

Returns identity and transaction info for a confirmed block
- **getProgramAccounts**: Provide the chain alias and program ID.

Returns all accounts owned by a program
- **getTransaction**: Provide the chain alias and transaction signature.

Returns details for a confirmed transaction
- **ankr_getTokenTransfers**: Supply the chain alias and the target address or token.

Returns historical token transfer data
- **eth_blockNumber**: Returns the most recent block number
- **eth_call**: Use this for pre-transaction validation.

Executes a call without creating a transaction
- **eth_getBlockByHash**: Use this to verify block existence.

Returns block information by hash
- **eth_getBalance**: Use this to check the available funds.

Returns the balance of an address
- **eth_getBlockByNumber**: Use this to check block history.

Returns block information by number
- **eth_getStorageAt**: Provide the contract address and storage slot.

Returns the value from a storage position
- **eth_getTransactionCount**: Use this value when constructing a new transaction.

Returns the number of transactions sent from an address (nonce)
- **getBalance**: Include both the chain alias and account Pubkey.

Returns the lamport balance of an account
- **getBlockHeight**: Only the chain alias is required.

Returns the current block height
- **getEpochInfo**: Specify the target chain alias.

Returns information about the current epoch
- **getLatestBlockhash**: Specify the target chain alias.

Returns the latest blockhash for transaction building
- **simulateTransaction**: Provide the chain alias and the transaction object.

Simulates a transaction to check for errors
- **sendTransaction**: Provide the chain alias and the signed transaction data.

Submits a signed transaction


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

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ankr-web3-node-api](https://vinkius.com/en/ai-agent-connect/ankr-web3-node-api)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `ankr-web3-node-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
