# Aurorascan (Aurora Network L2 Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aurorascan-aurora-network-l2-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Aurora Network L2 blockchain data—query balances, transaction history, and token transfers directly from your AI agent.

## Description
Connect your AI agent to **Aurorascan** and gain deep visibility into the Aurora Network L2 blockchain. This server enables real-time querying of account balances, transaction histories, and token movements through simple natural language.

### What you can do

- **Balance Inquiries** — Fetch Ether balances for single or multiple addresses simultaneously to monitor wallet health.
- **Transaction History** — Retrieve comprehensive lists of normal and internal transactions for any address, including block ranges and sorting.
- **Token Tracking** — Monitor ERC20, ERC721 (NFT), and ERC1155 transfer events to track asset movements and contract interactions.
- **Network Auditing** — List blocks mined by specific addresses to analyze network participation and validator activity.
- **Deep Data Inspection** — Access transaction hashes, contract addresses, and specific block parameters for granular blockchain analysis.

### How it works

1. Subscribe to this server
2. Enter your Aurorascan API Key
3. Start querying the Aurora L2 network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contract interactions and verify transaction statuses directly from your IDE.
- **Data Analysts** — Aggregate wallet balances and token transfer data without writing custom scripts.
- **Crypto Power Users** — Monitor personal portfolios and track specific on-chain events through a conversational interface.


## Available Tools (30)
- **proxy_get_code**: eth_getCode
- **proxy_get_storage_at**: eth_getStorageAt
- **proxy_get_transaction_by_hash**: eth_getTransactionByHash
- **proxy_get_transaction_receipt**: eth_getTransactionReceipt
- **verify_source_code**: Verify Source Code
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_no_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_eth_price**: Get Last Price of Ether in BTC and USD
- **get_eth_supply**: Get Total Supply of Ether on Aurora
- **get_logs**: Get Logs
- **get_mined_blocks**: Get list of Blocks Mined by Address
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_status**: Check Contract Execution Status
- **get_token_1155_tx**: Get a List of ERC1155 Token Transfer Events
- **get_token_balance**: Get ERC20-Token Balance for Address by ContractAddress
- **get_token_nft_tx**: Get a List of ERC721 Token Transfer Events
- **get_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_token_tx**: Get a List of ERC20 Token Transfer Events
- **get_tx_list_internal**: Get a List of Internal Transactions
- **get_tx_list**: Get a List of Normal Transactions By Address
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_block_number**: eth_blockNumber
- **proxy_call**: eth_call
- **proxy_estimate_gas**: eth_estimateGas
- **proxy_gas_price**: eth_gasPrice
- **proxy_get_block_by_number**: eth_getBlockByNumber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aurorascan (Aurora Network L2 Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance of address 0x123...?"

**🤖 AI Agent:**
> The current balance for address 0x123... is 4.52 ETH on the Aurora Network.

---

**👤 You:**
> "List the last 5 ERC20 token transfers for address 0xabc..."

**🤖 AI Agent:**
> I found the 5 most recent ERC20 transfers for that address. Notable transfers include 100 USDC and 50 AURORA tokens. Would you like the transaction hashes for these?

---

**👤 You:**
> "Show me the normal transaction history for address 0xdef... sorted by descending order."

**🤖 AI Agent:**
> Fetching transaction history... I've retrieved the latest transactions for 0xdef... including a contract interaction at block 1045231 and a simple transfer at block 1045220.


## ❓ FAQ

**Q: Can I check the balance of multiple wallet addresses at once?**
Yes. Use the `get_balance_multi` tool and provide a comma-separated list of addresses. The agent will return the Ether balance for all specified accounts in a single response.

**Q: How do I track NFT transfers for a specific user?**
You can use the `get_token_nft_tx` tool by providing the user's wallet address. This will list all ERC721 token transfer events associated with that address.

**Q: Does this server support internal transactions?**
Absolutely. The `get_tx_list_internal` tool allows you to query internal transactions by either a wallet address or a specific transaction hash.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aurorascan-aurora-network-l2-block-explorer-api](https://vinkius.com/mcp/aurorascan-aurora-network-l2-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aurorascan (Aurora Network L2 Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aurorascan-aurora-network-l2-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aurorascan (Aurora Network L2 Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aurorascan-aurora-network-l2-block-explorer-api": {
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
