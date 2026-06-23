# FtmScan (Fantom Network Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Fantom blockchain data directly—query wallet balances, transaction history, smart contract source code, and token transfers via FtmScan.

## Description
Connect to the **Fantom Network** through FtmScan to inspect on-chain activity using natural language. This server allows your AI agent to act as a blockchain explorer, providing real-time data on accounts, transactions, and smart contracts.

### What you can do

- **Account Analytics** — Retrieve FTM balances for single or multiple addresses and track transaction history (normal and internal).
- **Token Tracking** — Monitor ERC-20 and ERC-721 (NFT) transfer events across the network.
- **Smart Contract Inspection** — Fetch verified source code and ABIs for any deployed contract to understand its logic.
- **Transaction Status** — Check the execution status and receipts of specific transaction hashes.
- **Network Data** — Get the current FTM price, total supply, and block rewards.

### How it works

1. Subscribe to this server
2. Enter your FtmScan API Key
3. Start querying the Fantom blockchain from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly verify contract code and transaction statuses without leaving the IDE.
- **Crypto Analysts** — track whale movements and token distributions through simple conversation.
- **DeFi Users** — check wallet balances and recent activity across the Fantom ecosystem.


## Available Tools (19)
- **get_block_countdown**: Get Estimated Block Countdown Time
- **get_block_reward**: Get Block Rewards
- **get_contract_abi**: Get Contract ABI
- **get_contract_source_code**: Get Contract Source Code
- **get_erc20_token_balance**: Get ERC20 Token Balance for Address
- **get_erc20_token_supply**: Get ERC20 Token Total Supply
- **get_erc20_transfers**: Get List of ERC20 Token Transfer Events
- **get_erc721_transfers**: Get List of ERC721 Token Transfer Events
- **get_eth_block_number**: Get Latest Block Number (Proxy)
- **get_eth_transaction_by_hash**: Get Transaction by Hash (Proxy)
- **get_ftm_balance_multi**: Get FTM Balance for Multiple Addresses
- **get_ftm_balance**: Get FTM Balance for a Single Address
- **get_ftm_last_price**: Get FTM Last Price
- **get_ftm_total_supply**: Get Total Supply of FTM
- **get_internal_transactions**: Get List of Internal Transactions
- **get_logs**: Get Event Logs
- **get_normal_transactions**: Get List of Normal Transactions
- **get_transaction_receipt_status**: Check Transaction Receipt Status
- **get_transaction_status**: Check Transaction Execution Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FtmScan (Fantom Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current FTM balance of address 0xbbbb6a3601eeed31c8245938021fb3d10e7c51e2?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 1,250.45 FTM.

---

**👤 You:**
> "Show me the last 5 normal transactions for 0xbbbb6a3601eeed31c8245938021fb3d10e7c51e2 sorted by newest."

**🤖 AI Agent:**
> I've retrieved the 5 most recent normal transactions for that address. They include several transfers and contract interactions from the last few hours.

---

**👤 You:**
> "Get the verified source code for the contract at 0x04068da6a83afcfa0e13ba15a6696662335d5b75."

**🤖 AI Agent:**
> I have successfully retrieved the verified source code for the contract. It appears to be a SpookySwap LP token contract written in Solidity.


## ❓ FAQ

**Q: Can I check the balance of multiple wallets at once?**
Yes, use the `get_ftm_balance_multi` tool with a comma-separated list of addresses. The agent will return the FTM balance for each address in the list.

**Q: How do I see the source code of a smart contract?**
Use the `get_contract_source_code` tool with the contract's address. If the contract is verified on FtmScan, the agent will retrieve the source code and metadata.

**Q: How can I verify if a transaction was successful?**
Use the `get_transaction_status` tool with the transaction hash. It will return the execution status code directly from the Fantom network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ftmscan-fantom-network-explorer](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FtmScan (Fantom Network Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ftmscan-fantom-network-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FtmScan (Fantom Network Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ftmscan-fantom-network-explorer": {
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
