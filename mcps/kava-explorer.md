# Kava Explorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kava-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Kava blockchain — inspect accounts, track transactions (extrinsics), monitor blocks, and analyze validator performance via Subscan.

## Description
Connect your AI agent to the **Kava Network** through this comprehensive explorer server. Powered by Subscan, it provides deep visibility into on-chain data, from simple account balances to complex validator metrics.

### What you can do

- **Account Auditing** — Retrieve detailed account info, token balances, and historical rewards or slash events for any Kava address.
- **Transaction Tracking** — Query specific extrinsics by hash or index, or list recent transactions with advanced filtering by module and call.
- **Network Monitoring** — Fetch real-time block data, list recent blocks, and inspect system events emitted by the blockchain.
- **Staking & Governance** — Access a complete list of validators and drill down into specific validator performance and staking details.

### How it works

1. Subscribe to this server
2. Enter your Subscan API Key
3. Start querying Kava mainnet data directly from your favorite AI client

### Who is this for?

- **Web3 Developers** — Debug extrinsics and monitor events without leaving your terminal or code editor.
- **Crypto Analysts** — Extract account balances and reward history for financial reporting and research.
- **Node Operators** — Monitor validator status and network health through natural language queries.


## Available Tools
- **get_account_info**: Get basic information for a Kava account
- **get_account_reward_slash**: Get rewards and slashes for an account
- **get_account_token**: Get token balances for an account
- **get_block**: Get block details by height or hash
- **list_blocks**: Get a list of blocks
- **list_events**: Get a list of events with filtering options
- **get_extrinsic**: Get extrinsic details by hash or index
- **list_extrinsics**: Get a list of extrinsics
- **get_validator**: Get details for a specific validator
- **list_validators**: Get a list of validators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kava Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the balance and account info for Kava address kava1..."

**🤖 AI Agent:**
> I've retrieved the account info for kava1... The account currently holds 1,250 KAVA with a nonce of 42. Would you like to see the specific token balances as well?

---

**👤 You:**
> "What are the latest blocks on the Kava network?"

**🤖 AI Agent:**
> Fetching the most recent blocks... The latest block is #5,402,120, produced 6 seconds ago by validator 'KavaLabs'. There were 12 extrinsics in this block.

---

**👤 You:**
> "Check the rewards and slashes for address kava1..."

**🤖 AI Agent:**
> I found 15 reward events for this address in the last 24 hours, totaling 5.2 KAVA. No slash events were detected in the recent history.


## ❓ FAQ

**Q: Can I check the token balances for a specific Kava address?**
Yes! Use the `get_account_token` tool with the target Kava address to retrieve all token balances associated with that account.

**Q: How do I find details about a specific transaction or extrinsic?**
You can use the `get_extrinsic` tool by providing either the transaction hash or the extrinsic index (e.g., '123456-2').

**Q: Is it possible to monitor validator performance and staking status?**
Absolutely. Use `list_validators` to see the network-wide list, and `get_validator` with a specific address to see detailed performance and staking metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kava-explorer](https://vinkius.com/mcp/kava-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kava Explorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kava-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kava Explorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kava-explorer": {
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
