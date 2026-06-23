# Gnosisscan (Gnosis Chain Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Gnosis Chain data directly—query account balances, transaction history, and smart contract details via Gnosisscan.

## Description
Connect your AI agent to the **Gnosis Chain** through the Gnosisscan API. This server allows you to inspect the blockchain, track xDAI balances, and analyze transaction flows without leaving your chat interface.

### What you can do

- **Account Auditing** — Retrieve xDAI balances for single or multiple addresses instantly.
- **Transaction History** — List normal and internal transactions, including paginated results and block ranges.
- **Token Tracking** — Monitor ERC20 and ERC721 (NFT) transfer events for any specific address or contract.
- **Smart Contract Insights** — Fetch verified Contract ABIs and Source Code for deep technical analysis.
- **Network Stats** — Get real-time data on block rewards, gas prices, and GNO price metrics.

### How it works

1. Subscribe to this server
2. Enter your Gnosisscan API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly fetch ABIs or check transaction receipts without switching to a browser.
- **Data Analysts** — aggregate balance data and token movements across multiple Gnosis Chain addresses.
- **DeFi Users** — track personal portfolio movements and internal contract interactions through natural language.


## Available Tools (26)
- **get_account_balance_multi**: Get xDAI Balance for Multiple Addresses
- **get_account_balance**: Get xDAI Balance for a Single Address
- **get_account_minedblocks**: Get a List of Blocks Validated by Address
- **get_account_tokennfttx**: Get a List of ERC721 Token Transfer Events by Address
- **get_account_tokentx**: Get a List of ERC20 Token Transfer Events by Address
- **get_account_txlist_internal**: Get a List of Internal Transactions by Address
- **get_account_txlist**: Get a List of Normal Transactions By Address
- **get_block_bytime**: Get Block Number by Timestamp
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_contract_sourcecode**: Get Contract Source Code for Verified Source Codes
- **get_logs**: Get Event Logs
- **get_stats_ethsupply**: Get Total Supply of xDAI on Gnosis Chain
- **get_stats_gnoprice**: Get Last Price of Gnosis (GNO) and xDAI
- **get_tx_receiptstatus**: Check Transaction Receipt Status
- **get_tx_status**: Check Contract Execution Status
- **proxy_blocknumber**: eth_blockNumber Proxy
- **proxy_call**: eth_call Proxy
- **proxy_estimategas**: eth_estimateGas Proxy
- **proxy_gasprice**: eth_gasPrice Proxy
- **proxy_getblockbynumber**: eth_getBlockByNumber Proxy
- **proxy_getcode**: eth_getCode Proxy
- **proxy_getstorageat**: eth_getStorageAt Proxy
- **proxy_gettransactionbyhash**: eth_getTransactionByHash Proxy
- **proxy_gettransactionreceipt**: eth_getTransactionReceipt Proxy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gnosisscan (Gnosis Chain Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the xDAI balance of address 0x0000000000000000000000000000000000000000?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 0.00 xDAI on the Gnosis Chain.

---

**👤 You:**
> "List the last 5 normal transactions for address 0x123...456."

**🤖 AI Agent:**
> Fetching transaction history... I found the most recent transactions for that address, including a transfer of 10 xDAI and several contract interactions. Would you like details on a specific hash?

---

**👤 You:**
> "Get the ABI for the contract at 0x789...012."

**🤖 AI Agent:**
> I have retrieved the ABI for the requested contract. It includes functions like `transfer`, `balanceOf`, and `approve`. I can now help you format calls to this contract.


## ❓ FAQ

**Q: Can I check the balance of multiple Gnosis Chain addresses at once?**
Yes! Use the `get_account_balance_multi` tool and provide a comma-separated list of addresses to get all balances in a single request.

**Q: How do I see the ERC20 token transfer history for an account?**
You can use the `get_account_tokentx` tool. Simply provide the account address, and optionally a specific contract address, to list all relevant token movements.

**Q: Is it possible to retrieve the source code of a verified smart contract?**
Yes, the `get_contract_source_code` tool allows you to fetch the source code for any verified contract on Gnosisscan using its address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer](https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gnosisscan (Gnosis Chain Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gnosisscan-gnosis-chain-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gnosisscan (Gnosis Chain Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gnosisscan-gnosis-chain-explorer": {
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
