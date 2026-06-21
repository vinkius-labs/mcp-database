# Pinterest Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinterest-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage advertising and pins via Pinterest Ads — list campaigns, track analytics, and audit audiences directly from any AI agent.

## Description
Connect your **Pinterest Advertising** account to any AI agent and take full control of your visual discovery marketing through natural conversation.

### What you can do

- **Campaign & Ad Group Oversight** — List all campaigns and ad groups to maintain a clear view of your advertising structure.
- **Analytics Tracking** — Fetch detailed performance metrics for specific date ranges to monitor your ROI.
- **Content Management** — List boards and pins to verify your creative assets and organic presence.
- **Audience Auditing** — List saved audiences and product catalogs to ensure your targeting is optimal.
- **Keyword Analysis** — List keywords associated with specific ad groups to refine your search strategy.

### How it works

1. Subscribe to this server
2. Enter your Pinterest OAuth2 Access Token and Ad Account ID
3. Start managing your visual campaigns directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Digital Marketers** — quickly check campaign spend or performance metrics while reviewing marketing plans.
- **E-commerce Managers** — monitor product catalogs and audience targeting directly from your chat interface.
- **Content Creators** — verify pins and boards across multiple accounts without leaving your workflow.


## Available Tools
- **get_pinterest_analytics**: Get advertising analytics
- **get_pinterest_campaign**: Get details for a specific campaign
- **list_pinterest_ad_groups**: List ad groups
- **list_pinterest_ads**: List Pinterest ads
- **list_pinterest_audiences**: List saved audiences
- **list_pinterest_boards**: List Pinterest boards
- **list_pinterest_campaigns**: List Pinterest ad campaigns
- **list_pinterest_catalogs**: List product catalogs
- **list_pinterest_keywords**: List keywords for an ad group
- **list_pinterest_pins**: List Pinterest pins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinterest Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Pinterest ad campaigns."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active ones: 'Summer Sale 2026', 'New Collection Launch', and 'Brand Awareness'. Would you like analytics for any of these?

---

**👤 You:**
> "How much did we spend on Pinterest ads between 2026-10-01 and 2026-10-15?"

**🤖 AI Agent:**
> Total spend for that period was $1,245.50 across all campaigns, generating 45,000 impressions and 1,200 clicks.

---

**👤 You:**
> "Show me the pins from my 'Home Decor' board."

**🤖 AI Agent:**
> I've retrieved the pins from 'Home Decor'. There are 12 pins, including 'Modern Living Room Ideas' and 'Minimalist Kitchen Setup'. Would you like the details for any specific pin?


## ❓ FAQ

**Q: How do I find my Pinterest Ad Account ID?**
In your Pinterest Business account, go to the Ads Manager. Your Ad Account ID is usually visible in the URL or in the account settings section.

**Q: Can I see performance metrics for specific dates?**
Yes! Use the `get_pinterest_analytics` tool and provide the `start_date` and `end_date` parameters along with the columns (metrics) you wish to retrieve.

**Q: What metrics can I retrieve?**
Common metrics include SPEND_IN_DOLLAR, IMPRESSION, CLICKTHROUGH, REPIN, and TOTAL_CONCLICK. You can provide multiple metrics separated by commas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinterest-ads](https://vinkius.com/mcp/pinterest-ads)
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
3. Set Type to "SSE", enter `pinterest-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinterest Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinterest-ads": {
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
