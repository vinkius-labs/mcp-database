# Harmonyscan (Harmony One Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harmonyscan-harmony-one-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Harmony One blockchain data — query balances, transactions, smart contracts, and network status directly from your AI agent.

## Description
Connect your AI agent to the **Harmony One** network via Harmonyscan. This MCP server allows for deep inspection of the Harmony blockchain, from simple balance checks to complex smart contract analysis.

### What you can do

- **Account Data** — Fetch ONE balances for single or multiple addresses instantly using `get_balance` and `get_balance_multi`.
- **Transaction History** — List normal, internal, and HRC20 token transactions with full metadata via `get_tx_list` and `get_token_tx`.
- **Smart Contract Auditing** — Retrieve verified source code and ABIs for on-chain contracts with `get_source_code` and `get_abi`.
- **Network Insights** — Monitor block rewards, ONE supply, and current market prices using `get_one_supply` and `get_one_price`.
- **Transaction Status** — Verify execution and receipt status for any transaction hash with `get_status`.

### How it works

1. Subscribe to this server
2. Enter your Harmonyscan API Key
3. Start querying the Harmony blockchain from Claude, Cursor, or any MCP-compatible client

No more manual searching through block explorers. Your AI acts as a blockchain analyst, providing real-time data on addresses, contracts, and network health.

### Who is this for?

- **Web3 Developers** — quickly fetch contract ABIs and source code directly in your IDE to speed up integration.
- **Crypto Analysts** — automate the tracking of whale movements and token transfers across the Harmony ecosystem.
- **DeFi Users** — check transaction statuses and wallet balances through simple natural language commands.


## Available Tools (14)
- **get_abi**: Get Contract ABI
- **get_balance_multi**: Get ONE Balance for Multiple Addresses
- **get_balance**: Get ONE Balance for a Single Address
- **get_block_reward**: Get Block Rewards
- **get_logs**: Get Event Logs
- **get_one_price**: ONE Last Price
- **get_one_supply**: Total Supply of ONE
- **get_source_code**: Get Contract Source Code
- **get_status**: Check Transaction Execution Status
- **get_token_tx**: Get List of HRC20 Token Transfer Events
- **get_tx_list_internal**: Get List of Internal Transactions
- **get_tx_list**: Get List of Normal Transactions
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_request**: Execute standard JSON-RPC methods via proxy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harmonyscan (Harmony One Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current ONE balance for address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e?"

**🤖 AI Agent:**
> The current balance for that address is 1,250.45 ONE.

---

**👤 You:**
> "List the last 5 HRC20 token transfers for address 0x123..."

**🤖 AI Agent:**
> I've found the 5 most recent HRC20 transfers. They include 100 VIPER tokens received yesterday and 50 FOX tokens sent 2 hours ago. Would you like the full details for any of these?

---

**👤 You:**
> "Get the ABI and source code for the contract at 0x0809D4A52411430218Af7a6d8f17513E99770059."

**🤖 AI Agent:**
> I have retrieved the verified source code and ABI for the contract. It is a 'ViperSwap' liquidity pool contract compiled with Solidity 0.6.12. I can now help you analyze its functions or events.


## ❓ FAQ

**Q: Can I check the balance of multiple Harmony addresses at once?**
Yes! Use the `get_balance_multi` tool and provide a comma-separated list of addresses (up to 20). The agent will return the ONE balance for each address in a single response.

**Q: How do I verify if a specific transaction was successful or failed?**
You can use the `get_status` tool with the transaction hash. It returns a status code where '1' indicates success and '0' indicates failure, along with any available error messages.

**Q: Is it possible to retrieve the source code of a smart contract?**
Yes, provided the contract is verified on Harmonyscan. Use the `get_source_code` tool with the contract address to get the Solidity source code, compiler version, and optimization settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harmonyscan-harmony-one-block-explorer-api](https://vinkius.com/mcp/harmonyscan-harmony-one-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harmonyscan (Harmony One Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harmonyscan-harmony-one-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harmonyscan (Harmony One Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harmonyscan-harmony-one-block-explorer-api": {
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
