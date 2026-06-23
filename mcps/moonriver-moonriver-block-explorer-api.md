# Moonriver (Moonriver Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Query Moonriver blockchain data—blocks, transactions, account balances, and EVM tokens—directly from your AI agent.

## Description
Connect to the **Moonriver** network to inspect real-time blockchain activity. This server allows your AI agent to interact with the Moonriver Block Explorer API, providing deep insights into on-chain data without leaving your chat interface.

### What you can do

- **Block Exploration** — List recent blocks or fetch specific block details by height using `list_blocks` and `get_block`.
- **Transaction Tracking** — Query extrinsics (transactions) by address or hash to monitor network activity via `list_extrinsics` and `get_extrinsic`.
- **Account Analysis** — Retrieve balance information, metadata, and transfer history for any Moonriver address with `get_account_info` and `list_transfers`.
- **EVM Token Monitoring** — List ERC-20 and ERC-721 tokens and track their movements across the network using `list_evm_tokens`.
- **Network Metadata** — Get high-level information about the Moonriver network status with `get_metadata`.

### How it works

1. Subscribe to this server
2. Enter your Moonriver (Subscan-based) API Key
3. Start querying the Kusama-based parachain from Claude, Cursor, or any MCP client.

No more manually searching through block explorers. Your AI acts as a dedicated blockchain analyst.

### Who is this for?

- **Web3 Developers** — quickly verify transaction statuses and account balances without leaving the IDE.
- **Data Analysts** — extract block data and token transfer history for research and reporting.
- **Crypto Enthusiasts** — monitor wallet activity and network health through natural conversation.


## Available Tools (8)
- **get_account_info**: Get account details
- **get_block**: Get block details
- **get_extrinsic**: Get extrinsic details
- **get_metadata**: Get Moonriver network metadata
- **list_blocks**: Get a list of blocks
- **list_evm_tokens**: Get token list
- **list_extrinsics**: Get a list of extrinsics (transactions)
- **list_transfers**: Get account transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moonriver (Moonriver Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blocks on the Moonriver network."

**🤖 AI Agent:**
> I've retrieved the latest blocks. The most recent block is 5,120,450, produced by collator '0x...'. Would you like to see the details for a specific block height?

---

**👤 You:**
> "Get details for block number 5000000."

**🤖 AI Agent:**
> Inspecting block 5,000,000... It contains 12 extrinsics and was finalized on 2023-10-15. The state root is '0x...'. Do you want to list the extrinsics for this block?

---

**👤 You:**
> "Show me the list of EVM tokens available on Moonriver."

**🤖 AI Agent:**
> Fetching EVM tokens... I found several tokens including MOVR (Native), xcKSM, and various ERC-20 assets. Would you like to see the transfer history for a specific token?


## ❓ FAQ

**Q: Can I check the balance and metadata of a specific Moonriver address?**
Yes! Use the `get_account_info` tool by providing the wallet address. Your agent will return the current balance and associated account metadata.

**Q: How can I track token transfers for a specific user?**
Use the `list_transfers` tool with the user's address. It will retrieve the history of token transfers (ERC-20/ERC-721) for that specific account.

**Q: Is it possible to look up a transaction using its hash?**
Absolutely. Use the `get_extrinsic` tool and provide the transaction hash to get full details about that specific operation on the network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api](https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moonriver (Moonriver Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moonriver-moonriver-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moonriver (Moonriver Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moonriver-moonriver-block-explorer-api": {
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
