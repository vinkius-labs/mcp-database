# Ad4Game MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ad4game)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Digital advertising for games — manage offers, retrieve creatives, and audit ad inventory via AI.

## Description
Connect your **Ad4Game** publisher account to your AI agent to streamline your gaming advertising workflow. From synchronizing the latest high-payout offers to retrieving creative assets for your offer walls, your agent manages your ad inventory through natural conversation.

### What you can do

- **Offer Synchronization** — List all available advertising offers linked to your specific zones and affiliate ID
- **Creative Retrieval** — Fetch banners, videos, and other creative assets associated with specific gaming offers
- **Detailed Offer Audit** — Retrieve technical metadata for individual offers, including payout rates and targeting rules
- **Inventory Management** — Monitor your active zones and ensure your local offer database is always up-to-date
- **Campaign Insights** — Quickly identify the best-performing gaming offers to optimize your publisher revenue

### How it works

1. Subscribe to this server
2. Enter your Ad4Game API Key, Affiliate ID, and Zone ID
3. Start managing your gaming ad offers and assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Publishers** — manage offer walls and in-game ads more efficiently
- **Ad Ops Managers** — audit offer inventory and creative availability instantly
- **Developers** — integrate real-time offer syncing into gaming applications and platforms
- **Marketing Analysts** — monitor payout trends and offer variety across gaming categories


## Available Tools
- **list_offers**: List all available ad offers
- **get_offer_details**: Get details for a specific offer
- **get_creatives**: Fetch creatives for an offer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ad4Game** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all high-payout gaming offers for my zone."

**🤖 AI Agent:**
> I've retrieved the available offers. You have 5 premium gaming offers with payouts above $2.00 per conversion. Would you like to see the creative assets for these?


## ❓ FAQ

**Q: How do I sync all available offers?**
Use the `list_offers` tool. It will query the Ad4Game API for all offers currently active for your specified Zone ID and Affiliate ID.

**Q: What response formats does the Ad4Game API support?**
The Ad4Game Offers API natively supports retrieval of tracking offers and promotional assets in both XML and JSON formats.

**Q: Can I obtain creative data directly via API endpoints?**
Yes, by calling the `getCreatives` method with a corresponding offer ID, the agent gets direct links to banners, HTML assets, and video creatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ad4game](https://vinkius.com/mcp/ad4game)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ad4Game** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ad4game` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ad4Game** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ad4game": {
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
