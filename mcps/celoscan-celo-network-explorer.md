# Celoscan (Celo Network Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/celoscan-celo-network-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Celo network data via Celoscan — check account balances, track transactions, and inspect smart contracts directly from your AI agent.

## Description
Connect your **Celoscan** API key to any AI agent to explore the Celo blockchain with ease. Analyze addresses, verify contract code, and audit transaction history through natural language.

### What you can do

- **Account Insights** — Fetch CELO balances for single or multiple addresses instantly to monitor wallet holdings.
- **Transaction History** — Query normal and internal transactions, including ERC20 and ERC721 (NFT) transfer events for any address.
- **Smart Contract Auditing** — Retrieve verified contract ABIs and source code for deep technical inspection and debugging.
- **Network Monitoring** — Check blocks mined by specific addresses and verify the receipt status of any transaction hash.

### How it works

1. Subscribe to this server
2. Enter your Celoscan API Key
3. Start querying the Celo Network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly pull contract ABIs and source code into your IDE to understand protocol implementations.
- **Data Analysts** — export transaction histories and token movements for reporting and on-chain forensics.
- **Crypto Users** — monitor wallet balances and transaction statuses without leaving your chat interface.


## Available Tools (18)
- **get_erc20_token_balance**: Get ERC20-Token Account Balance by ContractAddress
- **get_erc20_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_account_balance**: Get CELO Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Smart Contracts
- **get_contract_source_code**: Get Contract Source Code for Verified Smart Contracts
- **get_account_balance_multi**: Get CELO Balance for Multiple Addresses
- **get_erc20_transfers**: Get a List of ERC20 Token Transfer Events By Address
- **get_erc721_transfers**: Get a List of ERC721 Token Transfer Events By Address
- **get_internal_transactions**: Get a List of Internal Transactions By Address
- **get_last_celo_price**: Get Last Price of CELO
- **get_mined_blocks**: Get list of Blocks Mined by Address
- **get_normal_transactions**: Get a List of Normal Transactions By Address
- **get_total_celo_supply**: Get Total Supply of CELO on the Celo Network
- **get_transaction_execution_status**: Check Contract Execution Status
- **get_transaction_receipt_status**: Check Transaction Receipt Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Celoscan (Celo Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the CELO balance for the address 0x1234567890abcdef1234567890abcdef12345678?"

**🤖 AI Agent:**
> The account balance for that address is 150.25 CELO.

---

**👤 You:**
> "List the recent ERC20 token transfers for address 0xabcdef..."

**🤖 AI Agent:**
> I found 5 recent ERC20 transfer events for that address. The most recent was a transfer of 50 cUSD from 0x789... to 0xabc... at block 12345678.

---

**👤 You:**
> "Get the ABI for the smart contract at 0x1234..."

**🤖 AI Agent:**
> I've retrieved the ABI for the contract. It contains functions such as `transfer`, `balanceOf`, and `approve`. Would you like me to explain any specific function?


## ❓ FAQ

**Q: Can I check the CELO balance of multiple addresses in a single request?**
Yes! Use the `get_account_balance_multi` tool and provide a comma-separated list of Celo addresses to retrieve all balances at once.

**Q: How can I view the source code of a verified smart contract on Celo?**
You can use the `get_contract_source_code` tool with the contract's address. If the contract is verified on Celoscan, the agent will return the full source code.

**Q: Is it possible to check if a specific transaction was successful?**
Yes, the `get_transaction_receipt_status` tool allows you to check the status of a transaction receipt to confirm if it was processed successfully on the network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/celoscan-celo-network-explorer](https://vinkius.com/mcp/celoscan-celo-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Celoscan (Celo Network Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `celoscan-celo-network-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Celoscan (Celo Network Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "celoscan-celo-network-explorer": {
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
