# Corescan (Core DAO Blockchain Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corescan-core-dao-blockchain-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Core DAO blockchain — check balances, track transactions, inspect smart contracts, and monitor network stats directly via AI.

## Description
Connect to **Corescan**, the premier block explorer for the Core DAO network, and empower your AI agent with real-time on-chain data. This server provides comprehensive access to the Core DAO ecosystem, allowing for deep analysis of accounts, tokens, and smart contracts.

### What you can do

- **Account Monitoring** — Retrieve CORE balances for single or multiple addresses (up to 20) in a single query.
- **Transaction History** — Fetch lists of normal and internal transactions, providing a clear view of wallet activity and smart contract interactions.
- **Token Tracking** — Monitor ERC20 and ERC721 (NFT) transfer events to track asset movements across the network.
- **Smart Contract Analysis** — Access verified source code and ABIs for smart contracts to understand their logic and interface.
- **Network Insights** — Check transaction statuses, block rewards, and total supply metrics to stay informed about the network's health.

### How it works

1. Subscribe to this server
2. Enter your Corescan API Key
3. Start querying the Core DAO blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Quickly inspect contract ABIs and source code without leaving your IDE.
- **Data Analysts** — Aggregate transaction data and monitor token flows for research or reporting.
- **Crypto Enthusiasts** — Keep track of your portfolio balances and transaction history through natural conversation.


## Available Tools (15)
- **get_account_balance_multi**: Get CORE balance for multiple addresses
- **get_account_balance**: Get CORE balance for a single address
- **get_block_countdown**: Get estimated block countdown time
- **get_block_reward**: Get block rewards by block number
- **get_contract_abi**: Get Contract ABI for verified source codes
- **get_contract_source_code**: Get Contract Source Code for verified source codes
- **get_erc20_transfers**: Get ERC20 token transfer events by address
- **get_erc721_transfers**: Get ERC721 token transfer events by address
- **get_internal_transactions**: Get a list of internal transactions by address
- **get_last_price**: Get CORE last price
- **get_logs**: Get event logs
- **get_normal_transactions**: Get a list of normal transactions by address
- **get_total_supply**: Get total supply of CORE
- **get_tx_receipt_status**: Check transaction receipt status
- **get_tx_status**: Check contract execution status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corescan (Core DAO Blockchain Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the CORE balance of address 0x393849...?"

**🤖 AI Agent:**
> The address 0x393849... currently holds 150.25 CORE on the Core DAO network.

---

**👤 You:**
> "List the last 5 normal transactions for address 0xabc123..."

**🤖 AI Agent:**
> I've retrieved the last 5 transactions for 0xabc123... The most recent was a transfer of 10 CORE to 0xdef... in block 1234567.

---

**👤 You:**
> "Get the ABI for the smart contract at 0x789ghi..."

**🤖 AI Agent:**
> I have successfully fetched the ABI for the contract at 0x789ghi... It includes functions like 'transfer', 'balanceOf', and 'mint'. Would you like me to explain any specific function?


## ❓ FAQ

**Q: Can I check the balance of multiple Core DAO addresses at once?**
Yes! Use the `get_account_balance_multi` tool and provide a comma-separated list of up to 20 addresses to get all balances in a single response.

**Q: How can I see the source code of a smart contract on Core DAO?**
You can use the `get_contract_source_code` tool with the contract's address. If the contract is verified on Corescan, the AI will retrieve the full source code for you.

**Q: Does this server support tracking NFT transfers?**
Absolutely. Use the `get_erc721_transfers` tool to list all NFT transfer events associated with a specific wallet address or contract.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corescan-core-dao-blockchain-explorer](https://vinkius.com/mcp/corescan-core-dao-blockchain-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corescan (Core DAO Blockchain Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corescan-core-dao-blockchain-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corescan (Core DAO Blockchain Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corescan-core-dao-blockchain-explorer": {
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
