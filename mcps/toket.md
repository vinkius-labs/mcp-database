# Toket MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/toket)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/toket-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/toket-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Accept crypto payments on your website with a checkout widget that supports Bitcoin, Ethereum, and major stablecoins.

## Description
Connect your **Toket** account to any AI agent and simplify how you deploy NFT collections, mint digital assets, and monitor blockchain interactions through natural conversation.

### What you can do

- **Collection Management** — List all your NFT collections and deploy new ERC-721 smart contracts instantly via AI.
- **Asset Minting** — Mint NFTs into specific collections or use 'Easy Mint' to quickly generate assets for recipients.
- **Transaction Oversight** — List and check the status of minting transactions to ensure successful blockchain delivery.
- **Gas Management** — Monitor your Gas Tank balance to keep your automated minting operations running smoothly.
- **Metadata Control** — Retrieve detailed metadata for collections and individual minted assets.
- **Blockchain Visibility** — Track the history of your digital asset distribution directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Toket API Key (found in your account dashboard)
3. Start managing your Web3 ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Marketers** — quickly mint rewards or loyalty NFTs for community members via simple AI commands.
- **NFT Project Owners** — monitor collection deployments and verify minting statuses across multiple chains.
- **Developers** — automate the creation of smart contracts and asset distribution directly from the workspace.


## Available Tools
- **create_collection**: Provide name, symbol, and owner wallet.

Create a new NFT collection
- **easy_mint**: Quickly mint an NFT
- **get_collection**: Get details of a specific collection
- **get_gas_tank_status**: Check Gas Tank balance
- **get_mint_status**: Get status of a minting transaction
- **list_collections**: List all NFT collections
- **list_mints**: List all minted NFTs
- **mint_nft**: Mint an NFT into a collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Toket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all NFT collections in my account."

**🤖 AI Agent:**
> I've retrieved your NFT collections. You have 3 active contracts: 'Vinkius Founders', 'Beta Access Pass', and 'Event Reward 2024'. Which one would you like to mint an asset into?

---

**👤 You:**
> "Mint a Founders NFT to the address '0x123...456'."

**🤖 AI Agent:**
> Minting initiated! I've triggered a new NFT creation for the Founders collection to the recipient 0x123...456. The transaction ID is mint_88231. I'll monitor its status on the blockchain for you.

---

**👤 You:**
> "Check the current status of my Gas Tank."

**🤖 AI Agent:**
> Fetching status... Your Gas Tank currently has 0.15 ETH (approx. 500 transactions). You have plenty of balance for upcoming automated minting operations.


## Installation & Usage

To install and use the **Toket** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/toket](https://vinkius.com/mcp/toket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
