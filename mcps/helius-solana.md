# Helius (Solana) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helius-solana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access high-performance Solana data—fetch assets, balances, transaction history, and priority fee estimates directly through your AI agent.

## Description
Connect your **Helius** account to any AI agent to interact with the Solana blockchain with unprecedented speed and depth. This server leverages Helius's powerful RPC and DAS (Digital Asset Standard) API to provide real-time blockchain intelligence.

### What you can do

- **Asset Management** — Fetch detailed metadata for NFTs, cNFTs, and fungible tokens using `get_asset` or `get_asset_batch`.
- **Wallet Intelligence** — Retrieve complete balances with real-time USD pricing using `get_wallet_balances` and track history with `get_wallet_history`.
- **Ownership Tracking** — List every asset owned by a specific Solana address via `get_assets_by_owner`.
- **Network Optimization** — Get precise priority fee estimates with `get_priority_fee_estimate` to ensure your transactions land during high congestion.
- **Advanced Search** — Query the blockchain for specific assets based on collection, creator, or attributes using `search_assets`.

### How it works

1. Subscribe to this server
2. Enter your Helius API Key
3. Start querying Solana data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contracts and verify on-chain state without leaving your IDE.
- **Crypto Analysts** — Perform deep wallet forensics and portfolio tracking through natural language.
- **NFT Collectors** — Manage and inspect compressed NFTs and collections with ease.


## Available Tools (14)
- **get_wallet_identity**: sol domains.

Resolve address to known entities
- **get_wallet_transfers**: Get incoming and outgoing token transfers
- **parse_transactions**: Parse raw transactions into human-readable data
- **search_assets**: Search for assets with advanced filtering
- **get_asset_batch**: Get multiple assets in one call
- **get_asset_proof**: Get Merkle proof for compressed NFTs
- **get_asset**: Get detailed data for a specific Solana asset
- **get_assets_by_owner**: List all assets owned by a wallet
- **get_priority_fee_estimate**: Recommended to provide the serialized transaction.

Get precise priority fee estimates
- **get_token_accounts**: Get all token accounts for a mint or owner
- **get_transaction_history**: Get enhanced transaction history for an address
- **get_wallet_balances**: Get token and NFT balances with USD values
- **get_wallet_funded_by**: Identify the original funding source of a wallet
- **get_wallet_history**: Get complete transaction history for a wallet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helius (Solana)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance and USD value of the wallet 86W9...?"

**🤖 AI Agent:**
> I've retrieved the balances for that wallet. It currently holds 15.5 SOL ($1,860), 500 USDC, and 3 NFTs. Total estimated value is $2,360.

---

**👤 You:**
> "List all NFTs owned by 6p6... including their metadata."

**🤖 AI Agent:**
> I found 12 assets for this owner. Notable items include 'Mad Lad #402' and 'Famous Fox #123'. Would you like the full metadata for any of these?

---

**👤 You:**
> "What is the recommended priority fee for a transaction right now?"

**🤖 AI Agent:**
> Based on current network conditions, the 'Medium' priority fee is approximately 5,000 micro-lamports. For urgent transactions, 'High' is recommended at 25,000 micro-lamports.


## ❓ FAQ

**Q: Can I see the USD value of my tokens and NFTs?**
Yes! Use the `get_wallet_balances` tool. It fetches native SOL, SPL tokens, and NFTs along with their current market pricing in USD.

**Q: How do I handle compressed NFTs (cNFTs)?**
You can use `get_asset` to see details or `get_asset_proof` to retrieve the Merkle proof required for on-chain interactions with compressed assets.

**Q: Can I search for assets by specific creators or collections?**
Absolutely. Use the `search_assets` tool with a JSON query to filter by collection ID, creator address, or specific attributes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helius-solana](https://vinkius.com/mcp/helius-solana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Helius (Solana)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `helius-solana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Helius (Solana)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "helius-solana": {
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
