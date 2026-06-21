# Suivision (Sui Blockchain Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Sui blockchain — query transactions, inspect accounts, analyze coins, and track on-chain objects directly from your AI agent.

## Description
Connect to the **Suivision API** to gain deep visibility into the Sui Network. This MCP server allows any AI agent to act as a powerful blockchain explorer, retrieving real-time data about transactions, account balances, and smart contract packages.

### What you can do

- **Transaction Analysis** — Fetch detailed metadata for any transaction digest or list recent network activity using `get_transaction` and `list_transactions`.
- **Account Insights** — Get comprehensive overviews of Sui addresses, including coin balances and owned objects (NFTs) via `get_account_overview` and `get_account_objects`.
- **Smart Contract Inspection** — Retrieve Move package details, bytecode, and transaction history for specific protocols using `get_package_details`.
- **Coin Metadata** — Access supply information and decimals for any coin type on the network with `get_coin_metadata`.

### How it works

1. Subscribe to this server
2. Enter your Suivision API Key
3. Start querying the Sui blockchain from Claude, Cursor, or any MCP-compatible client.

No more manual searching through web explorers. Your AI acts as a dedicated blockchain analyst, providing technical data in seconds.

### Who is this for?

- **Web3 Developers** — quickly inspect package bytecode and transaction effects without leaving the IDE.
- **Crypto Analysts** — track whale movements, account balances, and coin supply metrics through natural language.
- **DeFi Users** — verify transaction statuses and object ownership on the Sui network instantly.


## Available Tools
- **get_account_coins**: List all coins owned by an account
- **get_account_objects**: List all objects owned by an account
- **get_account_overview**: Get account overview and balance
- **get_account_transactions**: List transactions associated with a specific account address
- **get_checkpoint**: Get details of a specific checkpoint
- **get_coin_metadata**: Get metadata for a specific coin type
- **get_coin_supply**: Get total supply for a specific coin type
- **get_defi_stats**: Get Sui DeFi statistics
- **get_epoch**: Get details of a specific epoch
- **get_object_details**: Get details of a specific on-chain object
- **get_package_details**: Get details of a Move package
- **get_package_transactions**: List transactions that interacted with a package
- **get_transaction**: Get detailed information about a specific transaction
- **list_checkpoints**: List recent network checkpoints
- **list_epochs**: List recent network epochs
- **list_transactions**: Supports pagination and ordering.

List recent transactions on the Sui network
- **list_validators**: List current network validators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Suivision (Sui Blockchain Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 transactions on the Sui network."

**🤖 AI Agent:**
> I've retrieved the latest activity. Recent transactions include digests like `5A2b...` and `8Xz9...`. Would you like me to inspect the details of the most recent one?

---

**👤 You:**
> "What are the coin balances for the address 0x123...?"

**🤖 AI Agent:**
> Checking the account... This address holds 150.5 SUI and 2,000 USDC. I also found 3 other minor coin types. Should I list the metadata for these coins?

---

**👤 You:**
> "Get the metadata and supply for the SUI coin type."

**🤖 AI Agent:**
> The SUI coin (0x2::sui::SUI) has 9 decimals. The current total supply is approximately 10 billion. Is there another coin type you'd like to analyze?


## ❓ FAQ

**Q: Can I check the balance and owned objects of a specific Sui address?**
Yes! Use the `get_account_overview` tool to see the general balance or `get_account_objects` to list all objects, including NFTs, associated with that address.

**Q: How do I get the technical details of a specific transaction digest?**
Simply provide the transaction hash to the `get_transaction` tool. It will return the sender, gas usage, status, and execution effects.

**Q: Can I inspect the source code or modules of a Move package?**
Yes, use the `get_package_details` tool with the Package ID. It retrieves the Move bytecode and module information directly from the blockchain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api](https://vinkius.com/mcp/suivision-sui-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Suivision (Sui Blockchain Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `suivision-sui-blockchain-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Suivision (Sui Blockchain Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "suivision-sui-blockchain-explorer-api": {
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
