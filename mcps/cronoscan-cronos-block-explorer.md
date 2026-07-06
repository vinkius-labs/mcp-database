# Cronoscan (Cronos Block Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cronoscan-cronos-block-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Cronos blockchain data — check CRO balances, track transactions, inspect smart contracts, and monitor token transfers directly via AI.

## Description
Connect to **Cronoscan** to analyze the Cronos blockchain through natural conversation. This server provides a comprehensive suite of tools for developers, traders, and analysts to interact with Cronos network data without leaving their AI interface.

### What you can do

- **Account Analysis** — Check CRO balances for single or multiple addresses and retrieve detailed transaction histories (normal and internal).
- **Token Tracking** — Monitor ERC-20 and ERC-721 (NFT) transfer events, check specific token balances, and track total supply metrics.
- **Smart Contract Insights** — Fetch contract ABIs and verified source code for deep technical inspection and security auditing.
- **Network Monitoring** — Get real-time data on gas prices, block rewards, and the current market price of CRO.
- **Geth Proxy Support** — Execute standard Ethereum-compatible RPC calls like `eth_call`, `eth_getTransactionReceipt`, and `eth_estimateGas` for advanced interactions.

### How it works

1. Subscribe to this server
2. Enter your Cronoscan API Key
3. Start querying Cronos blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and inspect contract source code directly from your coding environment.
- **Crypto Analysts** — Track whale movements, monitor token distributions, and generate on-chain reports via chat.
- **DeFi Users** — Check your portfolio balances and transaction status across the Cronos ecosystem instantly.


## Available Tools (24)
- **get_balance_multi**: Get CRO Balance for Multiple Addresses
- **get_balance**: Get CRO Balance for a Single Address
- **get_eth_price**: Get CRO Last Price
- **get_eth_supply**: Get Total Supply of CRO on Cronos
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_logs**: Get Logs
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_eth_block_number**: Proxy: eth_blockNumber
- **proxy_eth_call**: Proxy: eth_call
- **proxy_eth_estimate_gas**: Proxy: eth_estimateGas
- **proxy_eth_gas_price**: Proxy: eth_gasPrice
- **proxy_eth_get_block_by_number**: Proxy: eth_getBlockByNumber
- **proxy_eth_get_code**: Proxy: eth_getCode
- **proxy_eth_get_storage_at**: Proxy: eth_getStorageAt
- **proxy_eth_get_transaction_by_hash**: Proxy: eth_getTransactionByHash
- **proxy_eth_get_transaction_receipt**: Proxy: eth_getTransactionReceipt
- **get_token_balance**: Get ERC20-Token Account Balance by ContractAddress
- **get_token_tx**: Get ERC20 Token Transfer Events by Address
- **get_tx_list_internal**: Get a List of Internal Transactions By Address
- **get_tx_list**: Get a List of Normal Transactions By Address
- **get_token_nft_tx**: Get ERC721 Token Transfer Events by Address
- **get_token_supply**: Get ERC20-Token Total Supply by ContractAddress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cronoscan (Cronos Block Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current CRO balance for address 0x690B9A9E9aa1C9dB991C7721a92d351Db4FaC990?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 1,250.45 CRO.

---

**👤 You:**
> "Show me the last 5 ERC-20 token transfers for 0x690B9A9E9aa1C9dB991C7721a92d351Db4FaC990."

**🤖 AI Agent:**
> I've retrieved the recent ERC-20 transfers. The most recent ones include 500 USDC and 100 VVS tokens. Would you like the transaction hashes for these?

---

**👤 You:**
> "Get the ABI for the contract at 0x5C7C6f200567e573C96E38557b2062993894f91a."

**🤖 AI Agent:**
> I have successfully fetched the ABI for that contract. It includes functions like `stake`, `withdraw`, and `claimRewards`. I can help you format a specific call if needed.


## ❓ FAQ

**Q: Can I check the CRO balance of multiple wallet addresses in a single request?**
Yes! Use the `get_balance_multi` tool by providing a comma-separated list of addresses. The AI will return the current balance for each address in the list.

**Q: How do I retrieve the source code of a verified smart contract on Cronos?**
You can use the `get_source_code` tool with the contract's address. If the contract is verified on Cronoscan, the AI will fetch the source code, compiler version, and other optimization details.

**Q: Is it possible to track NFT transfers for a specific user?**
Absolutely. Use the `get_token_nft_tx` tool with the user's wallet address. You can also filter by a specific NFT contract address to narrow down the results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cronoscan-cronos-block-explorer](https://vinkius.com/mcp/cronoscan-cronos-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cronoscan (Cronos Block Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cronoscan-cronos-block-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cronoscan (Cronos Block Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cronoscan-cronos-block-explorer": {
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
