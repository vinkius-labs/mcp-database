# Pinterest Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinterest-ads-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent with direct access to Pinterest Ads — manage campaigns, track pin performance, and optimize shopping ad spend without opening Pinterest Ads Manager.

## Description
Connect **Pinterest Ads** to your AI agent and manage your visual advertising campaigns conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause campaigns, ad groups, and promoted pins.
- **Performance Analytics** — Pull impressions, clicks, CTR, CPC, conversions, ROAS, and pin engagement.
- **Shopping Ads** — Monitor product catalog performance, shopping campaign metrics, and catalog sync status.
- **Audience Insights** — Query audience demographics, interests, and keyword-based targeting data.

### How it works

1. Subscribe to the Pinterest Ads integration on the marketplace.
2. Create an app in the Pinterest Developer Portal (developers.pinterest.com → My Apps → Create App).
3. Ask your AI agent to manage campaigns, check analytics, or optimize budgets.

### Who is this for?

- **E-commerce Brands** — Track shopping ad performance, product catalog metrics, and conversion attribution.
- **Visual Marketers** — Monitor pin engagement and optimize creative performance by audience segment.
- **Agencies** — Manage multiple client Pinterest ad accounts from a single conversational interface.


## Available Tools
- **list_campaigns**: List campaigns
- **list_adgroups**: List ad groups
- **list_ads**: List ads/Pins
- **get_campaign_analytics**: Get campaign analytics
- **get_adgroup_analytics**: Get ad group analytics
- **get_account_analytics**: Get account analytics
- **pause_campaign**: Pause campaign
- **enable_campaign**: Enable campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinterest Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How are my Pinterest shopping campaigns performing?"

**🤖 AI Agent:**
> 3 active shopping campaigns. Total spend this week: $2,100. Best performer: 'Spring Collection' (ROAS: 5.2x, 890 clicks, 67 checkouts). Catalog: 2,340 products synced, 98% approved.

---

**👤 You:**
> "Which pins have the highest engagement rate?"

**🤖 AI Agent:**
> Top 3 pins by engagement: 1) 'Minimalist Kitchen Ideas' (12.5% engagement, 4,200 saves), 2) 'Fall Wardrobe Essentials' (10.8%, 3,100 saves), 3) 'Home Office Setup Guide' (9.2%, 2,800 saves).

---

**👤 You:**
> "Increase the budget on 'Spring Collection' campaign by 20%."

**🤖 AI Agent:**
> Budget updated: 'Spring Collection' daily budget changed from $300 to $360 (+20%). Based on current performance (5.2x ROAS), the additional $60/day should generate approximately 19 more checkouts.


## ❓ FAQ

**Q: How do I get my Pinterest Ads API credentials?**
1. Go to **developers.pinterest.com** and log in with your Pinterest Business account.
2. Click **My Apps** → **Create App**.
3. Fill in the app name and description.
4. After creation, copy your **App ID** and **App Secret** from the app dashboard.
5. Generate an **Access Token** by authorizing your ad account.
6. Paste all values below.

💡 You need a **Pinterest Business Account** with an active ads account. Convert a personal account at [business.pinterest.com](https://business.pinterest.com).

**Q: Can I track shopping ad performance?**
Yes. Your AI agent tracks product-level metrics including impressions, clicks, add-to-carts, checkouts, ROAS, and catalog sync health — giving you real-time visibility into your Pinterest shopping campaigns.

**Q: What audience targeting is available?**
Pinterest supports interest targeting, keyword targeting, demographics (age, gender, location), device targeting, customer lists, website visitors (retargeting), actalike audiences, and shopping behavior targeting.

**Q: Is this useful for e-commerce brands?**
Absolutely. Pinterest is one of the highest-intent social platforms for shopping — 80% of weekly users have discovered a new brand or product on Pinterest. Your AI agent helps you maximize ROAS across product catalog campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinterest-ads-1](https://vinkius.com/mcp/pinterest-ads-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinterest Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pinterest-ads-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinterest Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinterest-ads-1": {
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
