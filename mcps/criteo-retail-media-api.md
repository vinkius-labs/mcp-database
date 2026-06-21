# Criteo Retail Media API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/criteo-retail-media-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent to manage Criteo retail campaigns, line items, and product data directly via the Criteo API.

## Description
Integrate the **Criteo Retail Media API** directly into your AI workflow. Manage your retail advertising campaigns, monitor line item performance, and track product data across your retailer and advertiser accounts using natural language.

### What you can do

- **Retail Campaign Management** — List and retrieve detailed settings for all your retail media campaigns.
- **Line Item Monitoring** — Access real-time configuration and performance for your retail line items.
- **Retailer & Product Discovery** — Explore retail partners and products associated with your advertiser accounts.
- **Keyword & Performance Insights** — Audit targeted keywords and request performance reports via chat.

### How it works

1. Connect the Criteo Retail Media integration to your AI assistant.
2. Authorize using your Criteo Client ID and Client Secret (found in the Criteo Developer Portal).
3. Orchestrate your retail media strategy through intuitive conversation.

### Who is this for?

- **Retail Media Managers** — Quickly check campaign statuses and retailer configurations on the go.
- **E-commerce Specialists** — Audit product placements and monitor line item performance via chat.
- **Account Executives** — Track advertiser accounts and retail partners during project planning.


## Available Tools
- **get_retail_campaign_details**: Get detailed settings for a specific retail campaign
- **get_retail_media_report**: Request a performance report for retail media
- **list_advertiser_accounts**: List advertiser accounts managed in retail media
- **list_retail_budgets**: List active budgets for retail media campaigns
- **list_retail_campaigns**: List all retail media campaigns in Criteo
- **list_line_item_keywords**: List keywords targeted by a specific line item
- **list_line_items**: List all line items (ad groups) for retail campaigns
- **list_account_products**: List products associated with a specific retail account
- **list_retailers**: List retail partners available in your account
- **search_retail_campaigns_by_name**: Search for retail campaigns by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Criteo Retail Media API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all retail media campaigns for advertiser account 'a8s9df7'."

**🤖 AI Agent:**
> I've found 3 campaigns for account 'a8s9df7', including 'Back to School 2024' and 'Electronics Spotlight'. Would you like to see the line items for any of these?

---

**👤 You:**
> "Show me the keywords being targeted in line item 'l123abc'."

**🤖 AI Agent:**
> Line item 'l123abc' is targeting 15 keywords, including 'laptop', 'gaming notebook', and 'ultrabook'. 5 of these keywords are currently generating conversions. Should I list the top performing ones?

---

**👤 You:**
> "Get a performance report for all retail campaigns from yesterday."

**🤖 AI Agent:**
> Yesterday, your retail campaigns generated 50,000 impressions and $5,000 in attributed sales across all retailers. The average ROAS was 4.5. Would you like a breakdown by retailer?


## ❓ FAQ

**Q: How do I get Criteo Retail Media API credentials?**
Log in to the Criteo Developer Portal, create a new app specifically for Retail Media, and you will receive a Client ID and Client Secret.

**Q: What is the difference between Marketing and Retail Media APIs?**
Marketing API focuses on off-site display and retargeting, while Retail Media API is designed for managing sponsored products and on-site advertising within retailer platforms.

**Q: Can I see keyword performance?**
Yes, you can use the list_line_item_keywords tool to see which keywords are being targeted and request reports to see their conversion metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/criteo-retail-media-api](https://vinkius.com/mcp/criteo-retail-media-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Criteo Retail Media API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `criteo-retail-media-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Criteo Retail Media API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "criteo-retail-media-api": {
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
