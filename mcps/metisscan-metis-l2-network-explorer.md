# Metisscan (Metis L2 Network Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metisscan-metis-l2-network-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Metis L2 network — inspect blocks, transactions, addresses, and smart contracts directly from your AI agent.

## Description
Connect your AI agent to the **Metis L2** ecosystem through Metisscan. Gain real-time visibility into the blockchain, from high-level network stats to granular smart contract data.

### What you can do

- **Network Monitoring** — List recent blocks and transactions or fetch the current block height using standard EVM methods.
- **Address Auditing** — Retrieve balances, transaction histories, and token holdings for any wallet or contract address.
- **Transaction Analysis** — Inspect transaction details, internal calls, and event logs to debug or track fund movements.
- **Smart Contract Insights** — Access contract source code, verification configurations, and interact with contracts via `eth_call` or `executeGraphql`.
- **Token Tracking** — List network tokens, check holders, and monitor transfers across the Metis Layer 2 ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Metisscan API Key
3. Start querying the Metis L2 network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and verify contract states without leaving your IDE.
- **Data Analysts** — Extract on-chain data and token metrics for research or reporting.
- **Crypto Power Users** — Track wallet activities and monitor network congestion through natural language.


## Available Tools
- **eth_block_number**: Get the most recent block number (RPC)
- **eth_call**: Execute a message call (RPC)
- **eth_estimate_gas**: Estimate gas for a transaction (RPC)
- **eth_get_balance**: Get address balance (RPC)
- **eth_get_block_by_number**: Get block by number (RPC)
- **eth_get_code**: Get code at address (RPC)
- **eth_get_transaction_by_hash**: Get transaction by hash (RPC)
- **eth_get_transaction_receipt**: Get transaction receipt (RPC)
- **get_address_counters**: g., transaction count) for a specific address.

Get transaction and token counters for an address
- **get_address_tokens**: List token balances for an address
- **get_address**: Get details for an address
- **get_address_transactions**: List transactions for an address
- **get_block**: Get details for a specific block
- **get_block_transactions**: List transactions in a block
- **get_smart_contract**: Get details for a smart contract
- **get_smart_contract_verification_config**: Get verification configuration for a smart contract
- **get_token_holders**: List token holders
- **get_token**: Get details for a specific token
- **get_token_transfers**: List token transfers
- **get_transaction_internal_transactions**: g., contract calls) triggered by a specific transaction.

List internal transactions for a transaction
- **get_transaction_logs**: List event logs for a transaction
- **get_transaction**: Get details for a specific transaction
- **graphql_query**: Execute a GraphQL query on Metisscan
- **list_blocks**: List recent blocks on Metis L2
- **list_tokens**: List tokens on the network
- **list_transactions**: List recent transactions on Metis L2


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metisscan (Metis L2 Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blocks on Metis L2."

**🤖 AI Agent:**
> I've retrieved the latest blocks. The most recent block is #12450672, containing 14 transactions. Would you like to see the transactions inside this block?

---

**👤 You:**
> "Get the transaction history for address 0xdead...beef."

**🤖 AI Agent:**
> I found 25 recent transactions for that address. The latest was a transfer of 5 METIS to a decentralized exchange 2 hours ago. Should I list the full details of the last 5 transactions?

---

**👤 You:**
> "Show me the source code and details for the smart contract at 0x123...456."

**🤖 AI Agent:**
> Accessing contract data... This is a verified 'TransparentUpgradeableProxy' contract. I have retrieved the ABI and the Solidity source code. Would you like me to analyze any specific function?


## ❓ FAQ

**Q: Can I check the balance and token holdings of a specific wallet address?**
Yes. Use the `getAddress` tool for the main balance and `getAddressTokens` to list all ERC-20 tokens held by that specific address on the Metis network.

**Q: How do I inspect the internal calls or logs of a specific transaction?**
You can use `getTransactionInternalTransactions` to see contract-to-contract interactions and `getTransactionLogs` to retrieve event data emitted during execution.

**Q: Is it possible to query the network using GraphQL or standard EVM RPC methods?**
Absolutely. This server includes `executeGraphql` for complex queries and a full suite of EVM tools like `ethBlockNumber`, `ethGetBalance`, and `ethCall`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metisscan-metis-l2-network-explorer](https://vinkius.com/mcp/metisscan-metis-l2-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metisscan (Metis L2 Network Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `metisscan-metis-l2-network-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metisscan (Metis L2 Network Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metisscan-metis-l2-network-explorer": {
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
