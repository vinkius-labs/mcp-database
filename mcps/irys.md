# Irys MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/irys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage permanent data storage on Irys — check storage prices, query transactions via GraphQL, and manage balances across multiple tokens.

## Description
Connect to **Irys**, the provenance layer for permanent data storage. This MCP server enables your AI agent to interact with Irys nodes to handle data uploads, verify storage costs, and explore historical transactions.

### What you can do

- **Storage Economics** — Use `get_price` to calculate exact costs for data storage in atomic units for tokens like Ethereum or Solana.
- **Data Discovery** — Search through permanent records using `query_transactions` with GraphQL filters for specific tags and values.
- **Account Oversight** — Monitor wallet balances with `get_balance` and manage node funding or withdrawals via `fund_account` and `withdraw_account`.
- **Transaction Metadata** — Retrieve detailed status and tags for any specific transaction ID using `get_transaction`.
- **Node Status** — Get real-time metadata about the Irys node configuration and supported features using `get_info`.

### How it works

1. Subscribe to this server
2. Provide your Irys Node URL (Mainnet or Devnet)
3. Start interacting with the permanent web through your AI agent

### Who is this for?

- **Web3 Developers** — quickly check upload prices and transaction statuses without leaving the terminal or IDE.
- **Data Analysts** — query historical data tags on the provenance layer to track on-chain activity.
- **DevOps Engineers** — automate the monitoring of Irys node balances and funding status.


## Available Tools (8)
- **get_info**: Get Irys node metadata
- **get_price**: Get storage price for a specific token and data size
- **query_transactions**: Use this to find historical transactions by tag.

Search and filter transaction metadata via GraphQL
- **submit_transaction**: Submit a signed data transaction
- **withdraw_account**: Initiate a withdrawal request
- **get_balance**: Get balance for a specific address
- **fund_account**: Submit a funding transaction receipt
- **get_transaction**: Retrieve metadata for a specific transaction ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Irys** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the storage price for 500MB using the solana token?"

**🤖 AI Agent:**
> I've checked the pricing for 500,000,000 bytes on Solana. The current cost is approximately 12,450,000 atomic units. Would you like to check the price for a different token?

---

**👤 You:**
> "Find the last 3 transactions with the tag 'App-Name' set to 'Vurb'."

**🤖 AI Agent:**
> I found 3 transactions matching your criteria. The most recent one has ID `zK9...` and was uploaded with the tag 'App-Name: Vurb'. Do you want the full metadata for any of these?

---

**👤 You:**
> "Show me the metadata and supported tokens for this Irys node."

**🤖 AI Agent:**
> Fetching node info... This node is running version 1.0.0 and supports tokens including ethereum, solana, arweave, and matic. It is currently healthy and accepting transactions.


## ❓ FAQ

**Q: How can I check the cost of storing a specific amount of data?**
Use the `get_price` tool by providing the payment token (e.g., 'ethereum') and the size in bytes. The agent will return the cost in atomic units for that specific network.

**Q: Is it possible to search for historical transactions by their tags?**
Yes! The `query_transactions` tool allows you to filter transactions using GraphQL by specifying a `tag_name` and `tag_value`, along with a result limit.

**Q: How do I verify the balance of a specific wallet on the Irys node?**
You can use the `get_balance` tool. Just provide the token type and the wallet address to retrieve the current balance held on the Irys node.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/irys](https://vinkius.com/mcp/irys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Irys** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `irys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Irys** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "irys": {
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
