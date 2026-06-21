# SolanaFM (Solana FM Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Solana blockchain data via SolanaFM — inspect blocks, transactions, account metadata, and token balances directly from any AI agent.

## Description
Connect to the **SolanaFM** block explorer API to empower your AI agent with deep indexing capabilities for the Solana network.

### What you can do

- **Block Exploration** — Fetch detailed block data or ranges using slot numbers via `get_block` and `get_blocks` tools.
- **Transaction Analysis** — Retrieve full transaction details via signatures with `get_transaction` or list all transactions for a specific address using `get_account_transactions`.
- **Account Intelligence** — Inspect account metadata, state, and ownership details using `get_account_info`.
- **Token Tracking** — List all token accounts owned by a specific wallet address with `get_token_accounts`.

### How it works

1. Subscribe to this server
2. Enter your SolanaFM API Key
3. Start querying Solana data from Claude, Cursor, or any MCP-compatible client

No more manual searching through web explorers. Your AI acts as a blockchain analyst, providing real-time data on accounts, blocks, and transactions.

### Who is this for?

- **Web3 Developers** — Debug transactions and verify account states straight from the code editor to avoid breaking flow.
- **Data Analysts** — Extract blockchain metrics and block history for research and reporting without complex scripts.
- **Crypto Enthusiasts** — Monitor wallet activity and token holdings through natural conversation.


## Available Tools
- **get_account_info**: Get the metadata and state of a Solana account
- **get_account_transactions**: List transactions associated with a specific account address
- **get_block**: Get detailed information about a specific block
- **get_blocks**: Get a list of blocks within a specified range
- **get_token_accounts**: Get token accounts owned by a specific wallet address
- **get_transaction**: Get details for a specific transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SolanaFM (Solana FM Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the details for Solana block at slot 250000000."

**🤖 AI Agent:**
> I've retrieved the details for block 250000000. It contains 2,450 transactions and was produced by validator 'Chorus One'. Would you like to see the list of transaction signatures in this block?

---

**👤 You:**
> "Show me all token accounts owned by 7xKX... (address)."

**🤖 AI Agent:**
> Analyzing the wallet... I found 3 token accounts for this address: 500 USDC, 1.5 SOL, and 10,000 BONK. Do you need the specific mint addresses for these tokens?

---

**👤 You:**
> "List the last transactions for account address 7xKX... (address)."

**🤖 AI Agent:**
> I've fetched the recent transaction history. There are 5 recent activities, including a 'Transfer' of 2 SOL and a 'Swap' on Jupiter. Would you like the full details for the most recent transaction signature?


## ❓ FAQ

**Q: How can I inspect the transaction history for a specific Solana wallet address?**
Use the `get_account_transactions` tool by providing the Solana account address. The agent will return a list of transactions associated with that specific wallet.

**Q: Can I see all the tokens held by a specific account?**
Yes! The `get_token_accounts` tool retrieves all token accounts owned by a target wallet address, allowing you to see balances and token types.

**Q: How do I get detailed information about a specific block on the Solana network?**
Simply use the `get_block` tool with the specific slot number. For a range of blocks, you can use the `get_blocks` tool with start and end slot numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api](https://vinkius.com/mcp/solanafm-solana-fm-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SolanaFM (Solana FM Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `solanafm-solana-fm-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SolanaFM (Solana FM Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solanafm-solana-fm-block-explorer-api": {
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
