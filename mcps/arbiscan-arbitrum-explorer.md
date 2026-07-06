# Arbiscan (Arbitrum Explorer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arbiscan-arbitrum-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore Arbitrum blockchain data — check balances, track transactions, and inspect smart contract source code directly from your AI agent.

## Description
Connect your AI agent to **Arbiscan** to query the Arbitrum L2 network in real-time. This MCP server allows you to fetch blockchain data without leaving your chat interface or IDE.

### What you can do

- **Account Auditing** — Check Ether balances for single or multiple addresses simultaneously.
- **Transaction Tracking** — Retrieve full history for normal, internal, ERC20, and ERC721 (NFT) transactions.
- **Contract Intelligence** — Fetch verified source code and ABIs to understand how dApps operate.
- **Network Insights** — Get real-time ETH price on Arbitrum, total supply, and block rewards.
- **Developer Tools** — Submit and verify contract source code directly through the API.

### How it works

1. Subscribe to this server
2. Enter your Arbiscan API Key
3. Start querying Arbitrum data from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Inspect contract ABIs and source code while writing code in your IDE.
- **Crypto Analysts** — Track whale movements and token transfers using natural language.
- **Security Researchers** — Quickly audit transaction history and internal calls for suspicious activity.


## Available Tools (16)
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_tx_list_internal**: Get List of Internal Transactions By Address
- **get_tx_list**: Get List of Normal Transactions By Address
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **verify_source_code**: Verify Source Code
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_status**: Check Contract Execution Status
- **get_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Arbitrum
- **get_logs**: Get Event Logs
- **get_token_nft_tx**: Get List of ERC721 Token Transfer Events By Address
- **get_token_tx**: Get List of ERC20 Token Transfer Events By Address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arbiscan (Arbitrum Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ETH balance of address 0x82aF49447D8a07e3bd95BD0d56f35241523fBab1?"

**🤖 AI Agent:**
> The address 0x82aF49447D8a07e3bd95BD0d56f35241523fBab1 currently holds 1,245.67 ETH on Arbitrum.

---

**👤 You:**
> "List the last 5 ERC20 token transfers for 0x123..."

**🤖 AI Agent:**
> I've retrieved the latest ERC20 transfers for that address. The most recent include 500 USDC from 0xabc... and 0.1 WETH to 0xdef.... Would you like the full transaction details?

---

**👤 You:**
> "Get the ABI for the contract at 0x912ce59144191c1204e64559fe8253a0e49e6548."

**🤖 AI Agent:**
> I have successfully fetched the ABI for the Arbitrum (ARB) token contract. It contains 24 functions, including `transfer`, `balanceOf`, and `delegate`. Do you need the JSON schema for a specific function?


## ❓ FAQ

**Q: Can I check the balances of multiple Arbitrum addresses at once?**
Yes! Use the `get_balance_multi` tool and provide a comma-separated list of addresses. The agent will return the Ether balance for each one in a single response.

**Q: How do I view the source code of a verified smart contract?**
Simply provide the contract address to the `get_source_code` tool. If the contract is verified on Arbiscan, your agent will retrieve the full source code for you to inspect.

**Q: Can I track NFT (ERC721) transfers for a specific wallet?**
Yes, the `get_token_nft_tx` tool allows you to list ERC721 token transfer events associated with any Arbitrum address, including block numbers and transaction hashes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbiscan-arbitrum-explorer](https://vinkius.com/mcp/arbiscan-arbitrum-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arbiscan (Arbitrum Explorer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arbiscan-arbitrum-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arbiscan (Arbitrum Explorer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arbiscan-arbitrum-explorer": {
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
