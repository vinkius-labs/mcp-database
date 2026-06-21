# Dogechain Explorer (Dogechain Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate Dogecoin blockchain analysis via Dogechain — check address balances, inspect transactions, and query block data directly from any AI agent.

## Description
Connect the **Dogechain** block explorer to your AI agent to monitor the Dogecoin network in real-time. Perform deep on-chain analysis, verify wallet balances, and track transaction flows through natural language.

### What you can do

- **Address Auditing** — Retrieve real-time balances, total coins received/sent, and transaction counts for any Dogecoin address.
- **Transaction Tracking** — Fetch detailed metadata for specific transaction hashes, including inputs, outputs, and confirmation status.
- **Block Inspection** — Query block data by height or hash and stay updated with the latest network activity using the best block hash tool.
- **UTXO Management** — List unspent transaction outputs (UTXOs) to understand wallet liquidity and prepare for transaction building.
- **Quick Validation** — Instantly check if a Dogecoin address is valid or decode it to its public key hash.

### How it works

1. Subscribe to this server
2. Enter 'public' or your Dogechain API key if applicable
3. Start querying the blockchain from Claude, Cursor, or any MCP-compatible client

No more manual searching on web explorers. Your AI acts as a blockchain analyst, providing raw data and insights directly in your workflow.

### Who is this for?

- **Crypto Traders & Whales** — Monitor wallet movements and verify large transactions without leaving your chat interface.
- **Blockchain Developers** — Debug transaction inputs/outputs and verify address balances during integration testing.
- **Data Analysts** — Extract on-chain metrics and block history for research and reporting.


## Available Tools
- **get_address_balance**: Get balance for a Dogecoin address
- **get_address_received**: Get total received amount for an address
- **get_address_sent**: Get total sent amount for an address
- **get_address_transaction_count**: Get transaction count for an address
- **get_address_transactions**: Results are paginated (10 per page).

Get recent transactions for an address
- **get_address_unspent**: Results are paginated (10 per page).

Get unspent outputs (UTXOs) for an address
- **get_best_block_hash**: Get the best block hash
- **get_block**: Get detailed block information
- **get_transaction**: Get detailed transaction information
- **q_address_balance**: Quick query: Get current balance
- **q_address_to_hash**: Quick query: Get public key hash
- **q_check_address**: Quick query: Check if address is valid
- **q_decode_address**: Quick query: Decode address
- **q_get_block_count**: Quick query: Get current block height
- **q_get_difficulty**: Quick query: Get last block difficulty
- **q_get_received_by_address**: Quick query: Get total amount ever received
- **q_get_sent_by_address**: Quick query: Get total amount ever sent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dogechain Explorer (Dogechain Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance of Dogecoin address D8v963B9wS4En543S8Z6eS6S6S6S6S6S6S?"

**🤖 AI Agent:**
> I've checked the address. The current balance for D8v963... is 1,250.50 DOGE (Confirmed: 1,250.50, Unconfirmed: 0.00).

---

**👤 You:**
> "Show me the details for transaction hash 76a4c8..."

**🤖 AI Agent:**
> Fetching transaction details... This transaction was included in block 4,500,123. It involved 2 inputs and 1 output, with a total value of 5,000 DOGE and 12 confirmations.

---

**👤 You:**
> "List the unspent outputs (UTXOs) for address D6r..."

**🤖 AI Agent:**
> I found 3 unspent outputs for address D6r... Totaling 450 DOGE. The largest UTXO is 300 DOGE from transaction hash b2f1...


## ❓ FAQ

**Q: Can I check the balance of a specific Dogecoin address?**
Yes! Use the `get_address_balance` tool with the target address. The agent will return the confirmed and unconfirmed balance immediately.

**Q: How do I find the latest block hash on the network?**
Simply ask the agent to run the `get_best_block_hash` action. It will retrieve the hash of the most recently mined block on the Dogecoin blockchain.

**Q: Is it possible to verify if a Dogecoin address is valid?**
Yes. Use the `q_check_address` tool. It provides a quick validation check to confirm if the provided string is a valid Dogecoin address format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api](https://vinkius.com/mcp/dogechain-explorer-dogechain-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dogechain Explorer (Dogechain Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dogechain-explorer-dogechain-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dogechain Explorer (Dogechain Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dogechain-explorer-dogechain-block-explorer-api": {
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
