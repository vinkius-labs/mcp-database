# TzKT (Tezos Indexer & Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access real-time Tezos blockchain data — explore accounts, smart contracts, and transaction history directly from your AI agent.

## Description
Connect to the **TzKT API**, the most advanced indexer for the Tezos blockchain. This MCP server allows your AI agent to query live on-chain data, analyze smart contract storage, and track financial operations across Mainnet and testnets.

### What you can do

- **Account Exploration** — List accounts by balance or activity and fetch detailed profiles including balance history.
- **Smart Contract Auditing** — Inspect contract code (Michelson/Micheline), current storage, and available entrypoints for any KT1 address.
- **Transaction Tracking** — Search operations by hash or list transactions with advanced filters like sender, target, and amount.
- **Financial Reporting** — Generate JSON-based activity reports for specific Tezos addresses.
- **Multi-Network Support** — Seamlessly switch between Mainnet, Ghostnet, and Shadownet.

### How it works

1. Subscribe to this server
2. (Optional) Enter your TzKT API Key for higher rate limits
3. Start querying the Tezos ledger from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contracts and verify storage states directly from your IDE.
- **Data Analysts** — Extract historical balance data and transaction flows for Tezos accounts.
- **DeFi Users** — Monitor wallet activity and track specific operation hashes without leaving the chat interface.


## Available Tools
- **get_account_balance_history**: Get historical balance changes for an account
- **get_account_report**: Generate a JSON report of account activity
- **get_account**: Get detailed information for a specific account
- **get_baker_rewards**: Get baker rewards per cycle
- **get_block**: Get block details by level or hash
- **get_contract_code**: Get contract Michelson or Micheline code
- **get_contract_entrypoints**: List available contract entrypoints
- **get_contract_storage**: Get current or historical contract storage
- **get_delegator_rewards**: Get delegator rewards per cycle
- **get_head**: Get the current state of the indexer and blockchain head
- **get_operations_by_hash**: Get operations by transaction hash
- **get_statistics**: Get network-wide statistics (TPS, volume, etc.)
- **list_accounts**: Supports filtering by balance, activity, and type.

List accounts with filters
- **list_bigmap_keys**: List keys in a specific big map
- **list_bigmap_updates**: Get update history for a big map
- **list_bigmaps**: List all big maps
- **list_blocks**: List blocks with filters
- **list_contracts**: List smart contracts with filters
- **list_delegations**: List delegation operations
- **list_originations**: List contract origination operations
- **list_staking**: List staking-related operations
- **list_token_balances**: Get token balances for specific accounts
- **list_token_definitions**: Get token metadata and definitions
- **list_token_transfers**: List token transfers (FA1.2 / FA2)
- **list_transactions**: List transactions with advanced filtering


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TzKT (Tezos Indexer & Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 5 accounts on Tezos mainnet with a balance greater than 1000 XTZ."

**🤖 AI Agent:**
> I've queried the mainnet accounts. Here are 5 accounts with balances over 1000 XTZ, including tz1... (Balance: 1500 XTZ) and tz1... (Balance: 1200 XTZ). Would you like to see the full report for any of these?

---

**👤 You:**
> "What are the available entrypoints for the smart contract KT1PWx2mnDuep3UMCcAgST9SetSjSEu7RZK1?"

**🤖 AI Agent:**
> I've retrieved the entrypoints for that contract. It features several callable functions including 'transfer', 'mint', 'burn', and 'set_metadata'. Which one would you like to inspect further?

---

**👤 You:**
> "Get the details for the Tezos transaction with hash ooVp... on Ghostnet."

**🤖 AI Agent:**
> Searching Ghostnet for operation ooVp... Found it! This was a transaction of 50 XTZ from tz1... to tz1... confirmed at block level 1,234,567. The status is 'applied'.


## ❓ FAQ

**Q: Can I see how an account's balance has changed over time?**
Yes! Use the `get_account_balance_history` tool with the account address. It will return a historical record of balance changes for that specific Tezos address.

**Q: How do I check the current state or storage of a smart contract?**
You can use the `get_contract_storage` tool by providing the contract's KT1 address. This will retrieve the current data stored in the contract's state.

**Q: Is it possible to list transactions for a specific sender or target?**
Absolutely. Use the `list_transactions` tool and apply filters like `sender` or `target` to narrow down the results to specific addresses or interaction flows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api](https://vinkius.com/mcp/tzkt-tezos-indexer-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TzKT (Tezos Indexer & Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tzkt-tezos-indexer-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TzKT (Tezos Indexer & Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tzkt-tezos-indexer-explorer-api": {
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
