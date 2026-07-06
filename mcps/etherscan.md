# Etherscan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/etherscan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query Ethereum and EVM-compatible blockchain data—check balances, transaction history, and token transfers directly from your AI agent.

## Description
Connect your **Etherscan** API key to any AI agent and gain instant access to on-chain data across Ethereum and other EVM-compatible networks through natural conversation.

### What you can do

- **Native Balances** — Retrieve the native token balance (ETH, MATIC, etc.) for single or multiple addresses (up to 20) using `get_balance` and `get_balance_multi`.
- **Transaction History** — Fetch comprehensive lists of normal and internal transactions for any wallet address with `get_tx_list` and `get_tx_list_internal`.
- **Token Tracking** — Monitor transfers for ERC-20, ERC-721 (NFTs), and ERC-1155 tokens using specialized tools like `get_token_tx` and `get_token_nft_tx`.
- **Multi-Chain Support** — Query data across different networks by specifying the `chainid` (e.g., 1 for Ethereum, 137 for Polygon).
- **Granular Filtering** — Filter transaction results by block range, pagination, and sort order to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your Etherscan API Key
3. Start auditing wallets and tracking transfers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contract interactions and verify transaction statuses directly from your IDE.
- **Crypto Analysts** — Track whale movements, token distributions, and wallet activity without manual block explorer searches.
- **DeFi Users** — Monitor your portfolio balances and transaction history through a simple chat interface.


## Available Tools (19)
- **get_balance_multi**: Get native token balances for multiple addresses
- **get_balance**: Get native token balance for an address
- **get_abi**: Get Contract ABI
- **get_address_tag**: Get address name tag (PRO Plus)
- **get_block_no_by_time**: Get block number by timestamp
- **get_block_number**: Get latest block number
- **get_eth_price**: Get Ether last price
- **get_eth_supply**: Get total supply of Ether
- **get_gas_oracle**: Get Gas Oracle
- **get_logs**: Get event logs
- **get_source_code**: Get Contract Source Code
- **get_transaction_by_hash**: Get transaction by hash
- **get_token_1155_tx**: Get ERC-1155 token transfers for an address
- **get_token_nft_tx**: Get ERC-721 token transfers for an address
- **get_token_tx**: Get ERC-20 token transfers for an address
- **get_tx_list_internal**: Get internal transactions for an address
- **get_tx_list**: Max 10,000 records.

Get normal transactions for an address
- **verify_source_code**: Verify Contract Source Code
- **get_address_token_balance**: Get address portfolio (PRO)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Etherscan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ETH balance of address 0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe on Ethereum?"

**🤖 AI Agent:**
> I've checked the balance for that address on Chain ID 1. The current balance is approximately 425.12 ETH (425123456789012345678 wei).

---

**👤 You:**
> "Show me the last 5 ERC-20 token transfers for 0x742d35Cc6634C0532925a3b844Bc454e4438f44e."

**🤖 AI Agent:**
> I've retrieved the ERC-20 transfer history. The most recent transfers include 500 USDT from 0xabc... and 100 LINK to 0xdef... Would you like more details on any of these transactions?

---

**👤 You:**
> "List the normal transactions for address 0x123... on Polygon (Chain ID 137)."

**🤖 AI Agent:**
> Querying Polygon scan... I found 10 recent transactions for that address. The latest was a contract interaction with Uniswap V3. Would you like me to list the specific transaction hashes?


## ❓ FAQ

**Q: How can I check the balance of multiple Ethereum addresses at once?**
You can use the `get_balance_multi` tool. Provide the `chainid` (e.g., 1 for Ethereum) and a comma-separated list of up to 20 addresses to retrieve all balances in a single request.

**Q: Can I track NFT transfers for a specific wallet?**
Yes! Use the `get_token_nft_tx` tool. By providing the wallet address and the appropriate `chainid`, the agent will list ERC-721 transfer events associated with that account.

**Q: Does this support networks other than Ethereum Mainnet?**
Yes, as long as you use the correct `chainid`. For example, use 1 for Ethereum, 137 for Polygon, or 10 for Optimism, provided your API key has access to those Etherscan-equivalent explorers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/etherscan](https://vinkius.com/mcp/etherscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Etherscan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `etherscan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Etherscan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "etherscan": {
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
