# Moonscan (Moonbeam Network Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moonscan-moonbeam-network-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Moonbeam blockchain data via Moonscan — check GLMR balances, track transactions, and inspect smart contracts directly from any AI agent.

## Description
Connect your **Moonscan** API key to any AI agent to explore the Moonbeam Network with ease. This server provides a comprehensive suite of tools for querying on-chain data without leaving your conversation.

### What you can do

- **Account Balances** — Retrieve GLMR balances for single or multiple addresses instantly.
- **Transaction History** — Fetch normal and internal transactions, including block ranges and sorting options.
- **Token Transfers** — Track ERC-20, ERC-721 (NFT), and ERC-1155 events for any address.
- **Contract Inspection** — Access verified smart contract ABIs and source code for deep analysis.
- **Status Checks** — Verify the receipt status of any transaction hash on the network.

### How it works

1. Subscribe to this server
2. Enter your Moonscan API Key
3. Start querying Moonbeam data from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Debug transactions and inspect contract code directly from your IDE.
- **Data Analysts** — Aggregate balance data and transfer events for on-chain research.
- **Crypto Enthusiasts** — Monitor wallet activity and token movements through natural language.


## Available Tools (26)
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards
- **get_contract_abi**: Get Contract ABI
- **get_contract_execution_status**: Check Contract Execution Status
- **get_contract_source_code**: Get Contract Source Code
- **get_erc1155_transfers**: Get List of ERC-1155 Token Transfer Events
- **get_erc20_balance**: Get ERC-20 Token Balance for Address
- **get_erc20_total_supply**: Get ERC-20 Token Total Supply
- **get_erc20_transfers**: Get List of ERC-20 Token Transfer Events
- **get_erc721_transfers**: Get List of ERC-721 (NFT) Token Transfer Events
- **get_glmr_balance_multi**: Get GLMR Balance for Multiple Addresses
- **get_glmr_balance**: Get GLMR Balance for a Single Address
- **get_glmr_last_price**: Get GLMR Last Price
- **get_glmr_total_supply**: Get Total Supply of GLMR
- **get_internal_transactions**: Get List of Internal Transactions
- **get_logs**: Get Logs
- **get_normal_transactions**: Get List of Normal Transactions
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_eth_block_number**: Proxy: eth_blockNumber
- **proxy_eth_call**: Proxy: eth_call
- **proxy_eth_estimate_gas**: Proxy: eth_estimateGas
- **proxy_eth_gas_price**: Proxy: eth_gasPrice
- **proxy_eth_get_block_by_number**: Proxy: eth_getBlockByNumber
- **proxy_eth_get_transaction_by_hash**: Proxy: eth_getTransactionByHash
- **proxy_eth_get_transaction_receipt**: Proxy: eth_getTransactionReceipt
- **get_block_countdown**: Get Estimated Block Countdown Time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moonscan (Moonbeam Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current GLMR balance for 0x21130d97301b6A5723dC95ca7519483491744ef1?"

**🤖 AI Agent:**
> The address 0x2113... currently holds 1,250.45 GLMR.

---

**👤 You:**
> "List the last 5 normal transactions for address 0x21130d97301b6A5723dC95ca7519483491744ef1 sorted by desc."

**🤖 AI Agent:**
> I've retrieved the 5 most recent transactions. The latest one was a transfer of 50 GLMR to 0xabc... at block 4,500,123.

---

**👤 You:**
> "Get the ABI for the smart contract at 0xacc15dc74880c9944775448304b263d191c6077f."

**🤖 AI Agent:**
> I have successfully retrieved the ABI for the contract. It includes functions like `transfer`, `balanceOf`, and `approve`. Would you like me to explain any specific function?


## ❓ FAQ

**Q: Can I check the GLMR balance of multiple wallets in a single request?**
Yes! Use the `get_glmr_balance_multi` tool and provide a comma-separated list of addresses to get all balances at once.

**Q: How do I view the verified source code of a Moonbeam smart contract?**
Simply use the `get_contract_source_code` tool with the contract address. If the contract is verified on Moonscan, the agent will retrieve the source code for you.

**Q: Is it possible to track NFT movements for a specific address?**
Yes, you can use `get_erc721_transfers` for standard NFTs or `get_erc1155_transfers` for multi-token standards to see all recent transfer events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonscan-moonbeam-network-explorer](https://vinkius.com/mcp/moonscan-moonbeam-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moonscan (Moonbeam Network Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moonscan-moonbeam-network-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moonscan (Moonbeam Network Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moonscan-moonbeam-network-explorer": {
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
