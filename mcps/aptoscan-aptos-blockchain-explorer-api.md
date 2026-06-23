# Aptoscan (Aptos Blockchain Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Aptos blockchain — check account balances, resources, transactions, and token data directly from your AI agent.

## Description
Connect to the **Aptoscan API** to inspect the Aptos blockchain in real-time. This MCP server allows any AI agent to query account states, transaction history, and token metadata without leaving the chat interface.

### What you can do

- **Account Insights** — Fetch balances, Move resources, and published modules for any Aptos address using `get_account_balance` and `get_account_resources`.
- **Transaction Tracking** — Retrieve detailed transaction data using hashes or ledger versions via `get_transaction_by_hash`.
- **Block Exploration** — Inspect specific blocks by height or transaction version to audit network activity.
- **Token & NFT Analysis** — List all tokens (NFTs and Fungible Assets) held by an account or fetch specific token metadata with `get_account_tokens`.
- **Developer Tools** — Access raw Move module data directly to analyze smart contract logic on-chain.

### How it works

1. Subscribe to this server
2. Enter your Aptoscan API Key
3. Start querying the Aptos ledger from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and inspect account resources without switching to a browser.
- **Data Analysts** — Pull on-chain data directly into your analysis workflow.
- **Crypto Enthusiasts** — Monitor wallet balances and NFT collections through natural conversation.


## Available Tools (10)
- **get_account_balance**: Get the current balance of the specified account
- **get_account_modules**: Get all Move modules published under the specified account
- **get_account_resources**: Get all resources owned by the specified account
- **get_account_tokens**: List all tokens (NFTs and Fungible Assets) held by an account
- **get_account_transactions**: Get a list of transactions associated with a specific account
- **get_block_by_height**: Get block details by its height
- **get_block_by_version**: Get block details containing a specific transaction version
- **get_token_data**: Get metadata and supply information for a specific token
- **get_transaction_by_hash**: Get details of a specific transaction using its hash
- **get_transaction_by_version**: Get details of a transaction using its ledger version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aptoscan (Aptos Blockchain Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance of the Aptos account 0x1?"

**🤖 AI Agent:**
> I'll check that for you. Using `get_account_balance` for address 0x1... The current balance is 100,000,000 APT.

---

**👤 You:**
> "List the last few transactions for address 0xeeff...8899."

**🤖 AI Agent:**
> Fetching transaction history using `get_account_transactions`... I found 10 recent transactions. The most recent was a 'User Transaction' at version 123456789.

---

**👤 You:**
> "Get block details for height 5000000."

**🤖 AI Agent:**
> Querying block data with `get_block_by_height`... Block 5000000 was proposed at timestamp 1690000000 and contains 45 transactions.


## ❓ FAQ

**Q: How do I check the balance of a specific Aptos wallet?**
Use the `get_account_balance` tool by providing the Aptos account address. The agent will return the current balance of that account immediately.

**Q: Can I see all NFTs and tokens owned by an address?**
Yes! The `get_account_tokens` tool lists all tokens, including NFTs and Fungible Assets, associated with a specific Aptos address.

**Q: How can I look up the details of a transaction if I have the hash?**
Simply use the `get_transaction_by_hash` tool with the transaction hash. It will retrieve full details including status, sender, and payload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api](https://vinkius.com/mcp/aptoscan-aptos-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aptoscan (Aptos Blockchain Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aptoscan-aptos-blockchain-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aptoscan (Aptos Blockchain Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aptoscan-aptos-blockchain-explorer-api": {
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
