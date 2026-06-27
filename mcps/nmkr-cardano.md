# NMKR Cardano MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nmkr-cardano)
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


## Available Tools (10)
- **get_mint_coupon_balance**: Check minting coupon balance
- **get_nft_details**: Get specific NFT metadata
- **get_project_counts**: Get project asset metrics
- **list_payout_wallets**: List all registered payout wallets
- **list_project_nfts**: List NFTs in a project
- **list_split_addresses**: List revenue split addresses
- **get_project_discounts**: List active project discounts
- **list_subcustomers**: List sub-customers for an account
- **list_vesting_addresses**: List vesting/staking addresses
- **validate_nft_metadata**: Validate NFT metadata


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


## ❓ FAQ

**Q: How do I get an NMKR Studio API Key?**
Log in to your NMKR Studio account and go to the API section in your profile settings to generate or copy your key.

**Q: Can I see the sales progress of my NFT collection?**
Yes! Use the `get_project_counts` tool with your Project UID to see how many NFTs have been sold, reserved, or remain free.

**Q: What does the metadata validation tool do?**
The `validate_nft_metadata` tool checks if your NFT metadata follows the CIP-25 standard for Cardano, ensuring it will display correctly on marketplaces and wallets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nmkr-cardano](https://vinkius.com/mcp/nmkr-cardano)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NMKR Cardano** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nmkr-cardano` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NMKR Cardano** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nmkr-cardano": {
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
