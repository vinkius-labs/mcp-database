# Snapchat Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snapchat-ads-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your Snapchat Ads campaigns — audit accounts, ad squads, and stats via AI.

## Description
Empower your AI agent to orchestrate your entire advertising ecosystem on Snapchat with **Snapchat Ads**, the platform for reaching the most engaged mobile audience. By connecting Snapchat Ads to your agent, you transform complex campaign management into a natural conversation. Your agent can instantly list your ad accounts, audit ad squad performance, and retrieve detailed analytics without you ever touching a dashboard. Whether you are scaling brand awareness or performance-driven ads, your agent acts as a real-time ad specialist, ensuring your marketing is always optimized and data-backed.

### What you can do

- **Account Auditing** — List all ad accounts associated with your organizations and retrieve detailed metadata for each.
- **Campaign Oversight** — List and audit campaigns, ad squads, and individual ads to maintain a structured view of your efforts.
- **Performance Intelligence** — Retrieve detailed advertising statistics with flexible dates to understand conversion and ROI.
- **Creative Governance** — List all media assets in your account to ensure your creative pipeline is healthy.
- **Organization Management** — Quickly retrieve organization-wide information to maintain strict control.

### How it works

1. Subscribe to this server
2. Enter your Snapchat Ads Access Token
3. Start managing your ad data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Buyers** — monitor daily spend and ad squad status straight from your workflow.
- **Marketing Leads** — verify if new creatives and campaigns have been correctly configured and are live.
- **Growth Analysts** — perform rapid audits of advertising performance and ROI without manual dashboard logins.
- **Business Owners** — automate ad querying to orchestrate your Snapchat-driven growth strategy smoothly.


## Available Tools
- **get_ad_account**: Get details for a specific ad account
- **list_organizations**: List Snapchat organizations
- **get_ad_account_stats**: Get statistics for an ad account
- **get_campaign_stats**: Get statistics for a campaign
- **list_ad_accounts**: List Snapchat ad accounts
- **list_ad_squads**: List ad squads for a campaign
- **list_ads**: List ads for an ad squad
- **list_campaigns**: List campaigns for an ad account
- **list_media**: List media assets for an ad account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snapchat Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Snapchat organizations."

**🤖 AI Agent:**
> I've retrieved your organizations. You have 2: 'Vinkius Global' and 'Media Team'. Which one would you like to audit for ad accounts?

---

**👤 You:**
> "Show me active campaigns for ad account ID xxxx."

**🤖 AI Agent:**
> I've found 3 active campaigns in that account: 'Spring Promo', 'App Install Drive', and 'Brand Reveal'. I can provide performance summaries for any of them.

---

**👤 You:**
> "Get an ads report for last month."

**🤖 AI Agent:**
> I've generated the report. Your total spend was $1,500 with 50,000 swipe-ups and an average cost per swipe of $0.03. Would you like a breakdown by campaign?


## ❓ FAQ

**Q: How do I find my Snapchat Ads Access Token?**
Create a Developer account at [**Snapchat Business**](https://business.snapchat.com/), create an App, and perform the OAuth flow to generate an Access Token. Copy and paste it below.

**Q: Can the agent list performance for specific ad squads?**
Yes. Use the `get_ad_account_stats` or similar tools providing the target ID and date range. Your agent will return metrics like swipe-ups, impressions, and spend.

**Q: Is it possible to audit creative media via the agent?**
Yes. The `list_media` tool allows your agent to retrieve all uploaded media assets and their metadata, ensuring your creative pipeline is ready for launch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snapchat-ads-alternative](https://vinkius.com/mcp/snapchat-ads-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Snapchat Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `snapchat-ads-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Snapchat Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "snapchat-ads-alternative": {
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
