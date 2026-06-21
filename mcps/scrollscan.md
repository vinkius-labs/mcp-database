# Scrollscan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scrollscan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Scroll L2 blockchain — check account balances, track transactions (normal, internal, ERC20/721/1155), and inspect contract ABIs directly from your AI agent.

## Description
Connect to **Scrollscan** and bring real-time Scroll L2 blockchain data into your AI-powered workflows. Whether you are debugging smart contracts or monitoring wallet activity, this server provides the essential tools for on-chain analysis.

### What you can do

- **Account Balances** — Fetch Ether balances for single or multiple addresses simultaneously
- **Transaction History** — Retrieve comprehensive lists of normal and internal transactions with block range filtering
- **Token Tracking** — Monitor transfer events for ERC20, ERC721 (NFTs), and ERC1155 tokens for any address
- **Contract Inspection** — Access verified contract ABIs to understand and interact with smart contracts
- **Network Insights** — List blocks mined by specific addresses and query internal transactions by hash

### How it works

1. Subscribe to this server
2. Enter your Scrollscan API Key
3. Start querying Scroll L2 data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug transaction flows and fetch contract ABIs directly from your code editor
- **Data Analysts** — aggregate on-chain activity and token movements without manual exports
- **Crypto Enthusiasts** — monitor portfolio balances and NFT transfers through natural conversation


## Available Tools (33)
- **check_verify_status**: Check Source Code Verification Status
- **get_account_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_account_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_contract_source_code**: Get Contract Source Code for Verified Source Codes
- **get_erc1155_token_tx**: Get ERC1155 Token Transfer Events by Address
- **get_erc20_token_tx**: Get ERC20 Token Transfer Events by Address
- **get_erc721_token_tx**: Get ERC721 Token Transfer Events by Address
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Scroll
- **get_internal_tx_list_by_block_range**: Get Internal Transactions by Block Range
- **get_internal_tx_list_by_hash**: Get Internal Transactions by Transaction Hash
- **get_internal_tx_list**: Get Internal Transactions by Address
- **get_logs**: Get Logs
- **get_mined_blocks**: Get List of Blocks Mined by Address
- **get_normal_tx_list**: Get Normal Transactions By Address
- **get_token_balance**: Get ERC20-Token Balance for Address by ContractAddress
- **get_token_supply**: Get ERC20-Token TotalSupply by ContractAddress
- **get_tx_receipt_status**: Check Check Transaction Receipt Status
- **get_tx_status**: Check Transaction Receipt Status
- **proxy_block_number**: eth_blockNumber
- **proxy_call**: eth_call
- **proxy_estimate_gas**: eth_estimateGas
- **proxy_gas_price**: eth_gasPrice
- **proxy_get_block_by_number**: eth_getBlockByNumber
- **proxy_get_code**: eth_getCode
- **proxy_get_storage_at**: eth_getStorageAt
- **proxy_get_transaction_by_hash**: eth_getTransactionByHash
- **proxy_get_transaction_receipt**: eth_getTransactionReceipt
- **verify_source_code**: Verify Source Code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scrollscan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ETH balance of address 0x1234567890abcdef1234567890abcdef12345678?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 1.25 ETH on the Scroll L2 network.

---

**👤 You:**
> "Show me the last 5 normal transactions for 0xabcdef..."

**🤖 AI Agent:**
> I've retrieved the transaction list using `get_normal_tx_list`. Here are the 5 most recent transactions, including hashes, block numbers, and values.

---

**👤 You:**
> "Get the ERC20 token transfer events for address 0x123... on contract 0x456..."

**🤖 AI Agent:**
> Searching for ERC20 transfers... I found several transfer events for that token contract associated with your address. Would you like the details for the most recent one?


## ❓ FAQ

**Q: How do I check the balance of multiple wallets at once?**
You can use the `get_account_balance_multi` tool. Simply provide a comma-separated list of addresses, and the agent will return the Ether balance for each one in a single request.

**Q: Can I track NFT transfers for a specific address?**
Yes! Use the `get_erc721_token_tx` tool for standard NFTs or `get_erc1155_token_tx` for multi-token standards. Provide the wallet address and the contract address to see all relevant transfer events.

**Q: How do I get the ABI for a verified contract?**
Use the `get_contract_abi` tool with the target contract address. If the source code is verified on Scrollscan, the agent will retrieve the complete ABI for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrollscan](https://vinkius.com/mcp/scrollscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scrollscan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scrollscan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scrollscan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrollscan": {
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
