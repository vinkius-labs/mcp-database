# Blastscan (Blast Network Explorer) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blastscan-blast-network-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blastscan-blast-network-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blastscan-blast-network-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Blast Network—check balances, track transactions, and inspect smart contracts directly from your AI agent.

## Description
Connect to **Blastscan**, the leading block explorer for the Blast Network, and empower your AI agent with real-time blockchain data and smart contract analysis.

### What you can do

- **Account Analytics** — Retrieve Ether and token balances for single or multiple addresses instantly.
- **Transaction Tracking** — List normal and internal transactions, as well as ERC20, ERC721, and ERC1155 transfer events.
- **Smart Contract Inspection** — Fetch verified source code and ABIs to understand contract logic and interactions.
- **Block & Network Data** — Query block rewards, estimated gas prices, and network-wide stats like ETH price and total supply.
- **Developer Proxy Tools** — Access low-level JSON-RPC proxy methods for deep chain state inspection, including storage slots and gas estimation.

### How it works

1. Subscribe to this server
2. Enter your Blastscan API Key
3. Start querying the Blast blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug transactions and verify contract states without leaving your IDE.
- **DeFi Power Users** — monitor wallet balances and token movements through natural language.
- **Security Researchers** — quickly pull contract source code and analyze internal transaction flows.


## Available Tools
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_ether_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_ether_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_eth_price**: Get Last Price of Ether
- **get_eth_supply**: Get Total Supply of Ether on Blast
- **get_logs**: Get Event Logs
- **get_mined_blocks**: Get list of Blocks Mined by Address
- **get_contract_source_code**: Get Contract Source Code for Verified Source Codes
- **get_erc1155_transfers**: Get a list of ERC1155 - Token Transfer Events by Address
- **get_erc20_token_balance**: Get ERC20-Token Account Balance by ContractAddress
- **get_erc721_transfers**: Get a list of ERC721 - Token Transfer Events by Address
- **get_erc20_token_supply**: Get ERC20-Token TotalSupply by ContractAddress
- **get_erc20_transfers**: Get a list of ERC20 - Token Transfer Events by Address
- **get_internal_transactions**: Get a list of Internal Transactions by Address
- **get_normal_transactions**: Get a list of Normal Transactions By Address
- **get_transaction_receipt_status**: Check Transaction Receipt Status
- **get_transaction_status**: Check Contract Execution Status
- **proxy_eth_blocknumber**: eth_blockNumber
- **proxy_eth_call**: eth_call
- **proxy_eth_estimategas**: eth_estimateGas
- **proxy_eth_gasprice**: eth_gasPrice
- **proxy_eth_getblockbynumber**: eth_getBlockByNumber
- **proxy_eth_getcode**: eth_getCode
- **proxy_eth_getstorageat**: eth_getStorageAt
- **proxy_eth_gettransactionbyhash**: eth_getTransactionByHash
- **proxy_eth_gettransactionreceipt**: eth_getTransactionReceipt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blastscan (Blast Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current ETH balance of address 0x0000000000000000000000000000000000000000 on Blast?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 1,250.45 ETH on the Blast Network.

---

**👤 You:**
> "List the last 5 normal transactions for address 0x123...abc."

**🤖 AI Agent:**
> Fetching transaction history... I found the 5 most recent transactions. The latest was a transfer of 0.5 ETH to 0xdef...789 at block 1234567. Would you like details on any specific transaction hash?

---

**👤 You:**
> "Get the ABI for the contract at 0x4300000000000000000000000000000000000004."

**🤖 AI Agent:**
> I have retrieved the ABI for the specified contract. It includes functions such as `yieldMode`, `configure`, and `claim`. I can now help you format calls to these functions.


## Installation & Usage

To install and use the **Blastscan (Blast Network Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blastscan-blast-network-explorer](https://vinkius.com/mcp/blastscan-blast-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
