# BlockCypher (Multi-chain Blockchain Developer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockcypher-multi-chain-blockchain-developer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access multi-chain blockchain data for BTC, ETH, and more. Query blocks, addresses, and transactions or broadcast new ones directly through AI.

## Description
Connect the **BlockCypher** multi-chain API to your AI agent to interact with major blockchains like Bitcoin, Ethereum, Litecoin, and Dogecoin through natural language.

### What you can do

- **Chain Monitoring** — Get real-time stats, block heights, and fee estimates for multiple blockchains and testnets
- **Address Auditing** — Query balances and transaction histories for any public wallet address without manual block explorer searches
- **Block Inspection** — Retrieve detailed block data by height or hash to analyze network activity
- **Wallet Generation** — Programmatically generate new public/private keypairs and addresses for supported coins
- **Transaction Management** — Create skeleton transactions, sign them, and broadcast them to the network directly from your agent
- **Real-time Webhooks** — Set up notifications for events like unconfirmed transactions or new blocks

### How it works

1. Subscribe to this server
2. Enter your BlockCypher API Token
3. Start querying blockchain data from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly check transaction statuses or generate testnet addresses without leaving the IDE
- **Crypto Analysts** — audit wallet balances and block data using natural language queries
- **Fintech Teams** — automate blockchain monitoring and transaction broadcasting workflows


## Available Tools
- **fund_bcy_test_address**: Fund an address on the BCY test chain
- **fund_beth_test_address**: Fund an address on the BETH test chain
- **call_eth_contract_method**: Requires token.

Call an Ethereum contract method
- **create_eth_contract**: Requires token.

Create an Ethereum contract
- **create_webhook**: Requires token.

Create a WebHook for real-time notifications
- **generate_address**: Requires token for POST.

Generate a new address and keypair
- **get_address_balance**: Get address balance only
- **get_address**: Get address details and transaction references
- **get_block_by_hash**: Get block details by hash
- **get_block_by_height**: Get block details by height
- **get_blockchain**: Get current state of a blockchain
- **get_transaction**: Get transaction details by hash
- **new_transaction**: Requires token for POST.

Create a skeleton transaction for signing
- **send_transaction**: Requires token for POST.

Send a signed transaction to the network
- **get_token_info**: Get information about an API token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlockCypher (Multi-chain Blockchain Developer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current status of the Bitcoin mainnet."

**🤖 AI Agent:**
> I've retrieved the Bitcoin mainnet status. The current height is 834,291 with a hash of 0000...a1b2. High priority fees are currently around 45 sat/vB.

---

**👤 You:**
> "Check the balance for BTC address 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa."

**🤖 AI Agent:**
> The address has a total balance of 99.98 BTC with 0 unconfirmed transactions.

---

**👤 You:**
> "Generate a new address for the Dogecoin testnet."

**🤖 AI Agent:**
> I've generated a new Dogecoin testnet address. Public Address: n1...xyz, Private Key: [hidden]. Make sure to save your private key securely.


## ❓ FAQ

**Q: Can I check the balance of a specific address without fetching all its transaction history?**
Yes! Use the `get_address_balance` tool. It provides a lightweight response containing only the balance and basic metadata for the specified coin and chain.

**Q: How do I find the current block height and fee estimates for Bitcoin?**
Simply use the `get_blockchain` tool with 'btc' as the coin and 'main' as the chain. It will return the latest block height, hash, and current network fee tiers.

**Q: Is it possible to generate a new wallet address for testing purposes?**
Yes. The `generate_address` tool allows you to create a new public/private keypair and address for any supported chain (e.g., 'btc' on 'test3' or 'bcy' on 'test').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockcypher-multi-chain-blockchain-developer-api](https://vinkius.com/mcp/blockcypher-multi-chain-blockchain-developer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlockCypher (Multi-chain Blockchain Developer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blockcypher-multi-chain-blockchain-developer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlockCypher (Multi-chain Blockchain Developer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blockcypher-multi-chain-blockchain-developer-api": {
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
