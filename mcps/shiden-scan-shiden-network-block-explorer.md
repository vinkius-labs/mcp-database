# Shiden Scan (Shiden Network Block Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore Shiden Network blockchain data—blocks, extrinsics, accounts, and EVM contracts—directly from your AI agent.

## Description
Connect to the **Shiden Network** (the multi-chain smart contract layer on Kusama) and query live blockchain data through natural language conversation.

### What you can do

- **Block & Extrinsic Tracking** — List recent blocks or fetch specific extrinsics by hash to monitor network activity and finality.
- **Account Auditing** — Retrieve detailed balance information (transferable, bonded, reserved) and transaction history for any SS58 address.
- **EVM Contract Inspection** — Fetch metadata and transaction logs for smart contracts deployed on Shiden's Ethereum-compatible layer.
- **Market Data** — Get real-time SDN token price, market capitalization, and 24h trading volume.
- **Network Metadata** — Access chain-specific details like token decimals, SS58 prefixes, and network naming conventions.

### How it works

1. Subscribe to this server
2. Enter your Shiden Scan (Subscan) API Key
3. Start querying the Shiden blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug extrinsics and verify contract deployments without leaving your code editor.
- **Crypto Analysts** — Track large transfers and monitor SDN market metrics via simple chat commands.
- **Node Operators** — Quickly check block heights and network metadata to ensure synchronization.


## Available Tools
- **get_account_info**: Retrieve balance and metadata for a specific account
- **get_block**: Retrieve details for a specific block
- **list_blocks**: Retrieve a list of blocks
- **get_evm_contract**: Retrieve information about a deployed smart contract
- **list_evm_transactions**: Retrieve transactions related to a specific contract
- **get_extrinsic**: Retrieve details for a specific extrinsic
- **list_extrinsics**: Retrieve a list of extrinsics
- **get_metadata**: Retrieve metadata about the Shiden Network
- **get_token_price**: Retrieve the current price of the SDN token
- **list_transfers**: Retrieve a list of transfers for a specific account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shiden Scan (Shiden Network Block Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blocks on the Shiden Network."

**🤖 AI Agent:**
> I've retrieved the latest blocks. The most recent block is #5,402,123, finalized with 12 extrinsics and 45 events. Would you like to see the details of a specific block number?

---

**👤 You:**
> "What is the current balance and status of address ab12...c34?"

**🤖 AI Agent:**
> For address ab12...c34, the total balance is 150.5 SDN. This includes 140.0 SDN transferable and 10.5 SDN bonded for staking. The account nonce is currently 42.

---

**👤 You:**
> "Show me the recent EVM transactions for the contract at 0x789...def."

**🤖 AI Agent:**
> I found 5 recent EVM transactions for that contract. The most recent one involved a 'Transfer' method call from 0xabc... to 0xdef... 2 minutes ago. Would you like to inspect the logs of a specific transaction?


## ❓ FAQ

**Q: Can I check the balance of a specific Shiden address?**
Yes! Use the `get_account_info` tool with the account address. The agent will return the transferable, bonded, and reserved balances, along with the account nonce.

**Q: How do I inspect a smart contract deployed on Shiden?**
You can use `get_evm_contract` to fetch general contract details or `list_evm_transactions` to see the recent transaction history for a specific contract address.

**Q: Can I see the current market price of the SDN token?**
Absolutely. The `get_token_price` tool retrieves the current price of SDN in USD and BTC, as well as its market cap and 24h volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer](https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shiden Scan (Shiden Network Block Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shiden-scan-shiden-network-block-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shiden Scan (Shiden Network Block Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shiden-scan-shiden-network-block-explorer": {
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
