# Bobascan (Boba L2 Network Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Boba L2 Network blockchain data — query balances, transaction histories, and smart contract ABIs directly from your AI agent.

## Description
Connect to the **Boba Network** (L2) through Bobascan's API. This MCP server allows your AI to act as a blockchain analyst, retrieving real-time data from the Boba L2 explorer.

### What you can do

- **Account Analysis** — Fetch Ether balances for single or multiple addresses on the Boba L2 network.
- **Transaction History** — List normal, internal, and token (ERC20/ERC721) transfer events for any wallet address.
- **Smart Contract Inspection** — Retrieve verified source code and ABIs to understand contract logic and interact with dApps.
- **Network Stats** — Get current gas prices, block rewards, and ETH price data directly from the chain.
- **Proxy Actions** — Perform low-level JSON-RPC calls like getting block numbers or transaction receipts.

### How it works

1. Subscribe to this server
2. Enter your Bobascan API Key
3. Start querying the Boba L2 network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly inspect contract ABIs and source code without leaving the IDE.
- **Data Analysts** — automate the retrieval of transaction lists and token transfers for reporting.
- **DeFi Users** — check wallet balances and transaction statuses through natural language.


## Available Tools (25)
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_execution_status**: Check Contract Execution Status
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Boba Network
- **get_ether_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_ether_balance**: Get Ether Balance for a Single Address
- **get_logs**: Get Logs
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_token_balance**: Get ERC20-Token Balance for Address by ContractAddress
- **get_token_nft_tx**: Get a List of ERC721 Token Transfer Events By Address
- **get_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_token_tx**: Get a List of ERC20 Token Transfer Events By Address
- **get_tx_list_internal**: Get a List of Internal Transactions By Address
- **get_tx_list**: Get a List of Normal Transactions By Address
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_block_number**: eth_blockNumber
- **proxy_call**: eth_call
- **proxy_estimate_gas**: eth_estimateGas
- **proxy_gas_price**: eth_gasPrice
- **proxy_get_block_by_number**: eth_getBlockByNumber
- **proxy_get_code**: eth_getCode
- **proxy_get_transaction_by_hash**: eth_getTransactionByHash
- **proxy_get_transaction_receipt**: eth_getTransactionReceipt
- **get_abi**: Get Contract ABI for Verified Source Codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bobascan (Boba L2 Network Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Ether balance of address 0x1234... on Boba L2?"

**🤖 AI Agent:**
> I've checked the balance for 0x1234... on the Boba Network. The current balance is 1.25 ETH.

---

**👤 You:**
> "List the last 5 transactions for address 0x5678..."

**🤖 AI Agent:**
> Fetching transaction history... I found the most recent transactions for 0x5678..., including a transfer of 0.5 ETH and several contract interactions. Would you like details on a specific hash?

---

**👤 You:**
> "Get the ABI for the smart contract at 0x9012..."

**🤖 AI Agent:**
> I have retrieved the ABI for the verified contract at 0x9012... You can now use this to decode transactions or prepare contract calls.


## ❓ FAQ

**Q: Can I check the Ether balance of multiple addresses at once?**
Yes! Use the `get_ether_balance_multi` tool and provide a comma-separated list of addresses to retrieve all balances in a single query.

**Q: How do I view the source code of a verified smart contract?**
You can use the `get_source_code` tool with the contract's address. If the contract is verified on Bobascan, the AI will return the Solidity source code.

**Q: Is it possible to track NFT transfers for a specific wallet?**
Yes, the `get_token_nft_tx` tool allows you to list ERC721 token transfer events associated with any address on the Boba network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api](https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bobascan (Boba L2 Network Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bobascan-boba-l2-network-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bobascan (Boba L2 Network Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bobascan-boba-l2-network-block-explorer-api": {
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
