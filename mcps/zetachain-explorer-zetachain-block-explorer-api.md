# Zetachain Explorer (ZetaChain Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zetachain-explorer-zetachain-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore ZetaChain blockchain data — inspect blocks, transactions, addresses, and tokens directly through any AI agent.

## Description
Connect to the **ZetaChain Explorer** and gain deep visibility into the ZetaChain network. This MCP server allows your AI agent to query real-time blockchain data, including transaction histories, smart contract details, and token balances.

### What you can do

- **Block & Transaction Monitoring** — List recent blocks and transactions, or fetch specific details using hashes or numbers.
- **Address Analysis** — Retrieve balances, token holdings, and transaction history for any wallet or contract address.
- **Smart Contract & Token Insights** — Inspect smart contract code, track token transfers, and list holders for specific assets.
- **Internal Operations** — Access internal transactions and event logs for comprehensive debugging and auditing.

### How it works

1. Subscribe to this server
2. Enter your ZetaChain API Key (optional)
3. Start querying the blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contracts and verify transaction logs directly from your IDE.
- **Data Analysts** — Extract token holder lists and transaction volumes without manual exports.
- **Crypto Enthusiasts** — Monitor wallet balances and network activity through natural conversation.


## Available Tools
- **get_block_transactions**: Get transactions in a specific block
- **get_block**: Get block details by hash or number
- **get_address_internal_transactions**: Get internal transactions for an address
- **get_address_token_balances**: Get token balances for an address
- **get_address_tokens**: Get tokens owned by an address
- **get_address**: Get address details
- **get_address_transactions**: Get transactions for an address
- **get_smart_contract**: Get smart contract details and ABI
- **get_token_holders**: Get token holders
- **get_token**: Get token details
- **get_token_transfers**: Get token transfers
- **get_transaction_internal**: g., contract calls) triggered by a specific transaction hash.

Get internal transactions for a specific transaction
- **get_transaction_logs**: Get logs for a specific transaction
- **get_transaction**: Get transaction details by hash
- **list_blocks**: List recent blocks on ZetaChain
- **list_tokens**: List tokens on ZetaChain
- **list_transactions**: List recent transactions on ZetaChain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zetachain Explorer (ZetaChain Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blocks on ZetaChain."

**🤖 AI Agent:**
> I've retrieved the latest blocks. The most recent block is #5829102, mined 12 seconds ago with 45 transactions. Would you like to see the transactions for a specific block?

---

**👤 You:**
> "Show me the token balances for address 0x1234...abcd."

**🤖 AI Agent:**
> For address 0x1234...abcd, I found balances for 3 tokens: 150 ZETA, 0.5 WETH, and 1,200 USDC. Would you like to see the recent transaction history for this address?

---

**👤 You:**
> "Get the event logs for transaction 0xabc123..."

**🤖 AI Agent:**
> I've fetched the logs for transaction 0xabc123... It emitted 2 events: a 'Transfer' event from the USDC contract and a 'Swap' event from the DEX router. Do you need the decoded parameters for these logs?


## ❓ FAQ

**Q: Can I inspect the internal calls triggered by a specific transaction?**
Yes. Use the `get_transaction_internal` tool with the transaction hash to retrieve all internal contract calls and operations associated with that transaction.

**Q: How do I check all token balances for a specific wallet address?**
Simply provide the wallet address to the `get_address_token_balances` tool. It will return a comprehensive list of all tokens held by that address on ZetaChain.

**Q: Is it possible to view the source code or ABI of a smart contract?**
Yes, the `get_smart_contract` tool allows you to fetch the metadata and details of a verified smart contract using its address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zetachain-explorer-zetachain-block-explorer-api](https://vinkius.com/mcp/zetachain-explorer-zetachain-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zetachain Explorer (ZetaChain Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zetachain-explorer-zetachain-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zetachain Explorer (ZetaChain Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zetachain-explorer-zetachain-block-explorer-api": {
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
