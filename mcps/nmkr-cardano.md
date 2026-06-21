# NMKR Cardano MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nmkr-cardano)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nmkr-cardano-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nmkr-cardano-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage Cardano NFT projects via NMKR Studio — track assets, minting coupons, and payout wallets directly from your AI agent.

## Description
Connect your **NMKR Studio** account to your AI agent and manage your Cardano NFT ecosystem through natural conversation using their powerful v2 API.

### What you can do

- **Asset Tracking** — List and inspect all NFTs within your projects, filtered by state (free, reserved, sold).
- **Project Metrics** — Retrieve real-time counts of sold and available NFTs and monitor active project discounts.
- **Financial Oversight** — Access your registered payout wallets and check your minting coupon balances.
- **Customer Management** — List and manage sub-customer profiles associated with your primary account.
- **Validation Tools** — Verify the compliance of your NFT metadata against Cardano standards.
- **Advanced Wallet Features** — Monitor active vesting (staking) and revenue split addresses.
- **Deep Inspection** — Fetch complete metadata and current state for specific NFTs using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your NMKR Studio API Key
3. Start managing your Cardano assets from Claude, Cursor, or any MCP client

### Who is this for?

- **NFT Creators & Artists** — quickly check the sales progress of a collection or validate metadata before minting.
- **Web3 Developers** — automate the retrieval of project metrics and wallet configurations through natural language.
- **Project Managers** — monitor sub-customers and revenue sharing arrangements directly from your workspace.


## Available Tools
- **validate_nft_metadata**: Validate NFT metadata
- **get_mint_coupon_balance**: Check minting coupon balance
- **get_nft_details**: Get specific NFT metadata
- **get_project_counts**: Get project asset metrics
- **get_project_discounts**: List active project discounts
- **list_payout_wallets**: List all registered payout wallets
- **list_project_nfts**: List NFTs in a project
- **list_split_addresses**: List revenue split addresses
- **list_subcustomers**: List sub-customers for an account
- **list_vesting_addresses**: List vesting/staking addresses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NMKR Cardano** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all payout wallets registered in my NMKR account."

**🤖 AI Agent:**
> Retrieving wallets... I found 2 registered payout addresses: one primary wallet (addr1...) and one secondary wallet for royalties. Would you like to check the current balance of your minting coupons as well?

---

**👤 You:**
> "What is the sales status for NFT project UID 'prj_12345'?"

**🤖 AI Agent:**
> Fetching project metrics... For project prj_12345, you have sold 150 NFTs, 25 are currently reserved, and 325 remain free for purchase. Shall I list the metadata for the most recently sold NFT?

---

**👤 You:**
> "Show me the metadata for the NFT with ID 'nft_98765'."

**🤖 AI Agent:**
> Inspecting NFT metadata... This asset is titled 'Space Traveler #42'. It is currently in the 'sold' state and its IPFS link is valid. All metadata fields follow the CIP-25 standard. Would you like to see the full JSON attributes?


## Installation & Usage

To install and use the **NMKR Cardano** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nmkr-cardano](https://vinkius.com/mcp/nmkr-cardano)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
