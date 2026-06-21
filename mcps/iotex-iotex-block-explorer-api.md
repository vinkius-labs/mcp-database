# IoTeX (IoTeX Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iotex-iotex-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access IoTeX blockchain data — query accounts, blocks, transactions, and token details directly from your AI agent.

## Description
Connect to the **IoTeX** blockchain and explore real-time network data through natural conversation. This MCP server provides a comprehensive interface to the IoTeX Block Explorer API.

### What you can do

- **Account Insights** — Retrieve balances, nonces, and metadata for any IoTeX address using the `get_account` tool.
- **Transaction History** — Fetch a list of actions associated with an account via `get_account_actions` or inspect specific transactions with `get_action`.
- **Block Exploration** — Query detailed block data by height or hash using `get_block_by_height` and `get_block_by_hash`.
- **Network Activity** — Monitor the pulse of the network with `get_recent_actions` to see the latest transactions.
- **Token Analysis** — Get metadata for XRC20/XRC721 tokens and list their holders using `get_token` and `get_token_holders`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your IoTeX API Key for higher rate limits
3. Start querying the IoTeX network from Claude, Cursor, or any MCP-compatible client

No more manual searching through web explorers. Your AI acts as a blockchain analyst, providing instant data on addresses, blocks, and tokens.

### Who is this for?

- **Web3 Developers** — quickly verify transaction statuses and account balances without leaving the code editor.
- **Data Analysts** — extract block and token holder data for research and reporting.
- **Crypto Enthusiasts** — monitor network activity and token metadata through simple chat commands.


## Available Tools (8)
- **get_account_actions**: Get Account Transactions
- **get_account**: Get Account Details
- **get_action**: Get Action by Hash
- **get_block_by_hash**: Get Block by Hash
- **get_block_by_height**: Get Block by Height
- **get_recent_actions**: Get Recent Actions
- **get_token_holders**: Get Token Holders
- **get_token**: Get Token Details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IoTeX (IoTeX Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get account details and balance for IoTeX address io1prv56hmvfm08z6p6v6v6v6v6v6v6v6v6v6v6v6."

**🤖 AI Agent:**
> I've retrieved the details for account io1prv... The current balance is 1,250 IOTX with a nonce of 42. Would you like to see the recent transaction history for this address?

---

**👤 You:**
> "Show me the most recent actions on the IoTeX network."

**🤖 AI Agent:**
> Fetching recent network activity... I found the latest actions including several transfers and contract executions. The most recent was a transfer of 500 IOTX at block height 31054201.

---

**👤 You:**
> "What are the details for the token at contract address io1hp6y4...?"

**🤖 AI Agent:**
> Analyzing token metadata... This contract corresponds to the 'MachineFi' token (MFI). It has a total supply of 1,000,000,000 and 18 decimals. Should I list the current top holders?


## ❓ FAQ

**Q: How can I see the transaction history for a specific IoTeX address?**
You can use the `get_account_actions` tool. Simply provide the IoTeX address, and the agent will return a list of recent actions (transactions) associated with that account.

**Q: Can I look up block details if I only have the block height?**
Yes! Use the `get_block_by_height` tool and provide the numeric height. The agent will fetch the full block details including hash, timestamp, and transaction count.

**Q: Is it possible to see who the top holders of a specific token are?**
Yes, by using the `get_token_holders` tool with the token's contract address, you can retrieve a list of addresses that currently hold that specific XRC20 or XRC721 token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iotex-iotex-block-explorer-api](https://vinkius.com/mcp/iotex-iotex-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IoTeX (IoTeX Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `iotex-iotex-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IoTeX (IoTeX Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "iotex-iotex-block-explorer-api": {
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
