# LinkedIn Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access marketing analytics, campaigns, and reporting via the LinkedIn Ads REST API.

## Description
Connect your **LinkedIn Ads** account to any AI agent to automate your professional marketing analytics and reporting. This MCP server enables your agent to list ad accounts, monitor campaign performance (impressions, clicks, spend), and retrieve conversion data directly from natural language interfaces using the latest LinkedIn REST API version.

### What you can do

- **Account Discovery** — List all accessible ad accounts and retrieve their current status and IDs
- **Campaign Monitoring** — Query campaign groups and individual campaigns to track your marketing objectives
- **Performance Querying** — Retrieve real-time performance metrics like impressions, clicks, and cost across various pivots (Account, Campaign, Creative)
- **Creative Oversight** — List and inspect individual ad variations and their technical configurations
- **Conversion Tracking** — Retrieve definitions for conversion rules to monitor your return on ad spend (ROAS)

### How it works

1. Subscribe to this server
2. Enter your LinkedIn Access Token (with required scopes) and API Version
3. Start managing your professional advertising metrics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance Marketers** — Monitor campaign spend and performance trends via simple natural language commands
- **Data Analysts** — Automate the extraction of LinkedIn advertising data into your reporting workflows
- **Growth Engineers** — Integrate advertising metadata and performance logs directly into your development tools


## Available Tools (6)
- **list_ad_accounts**: List all accessible LinkedIn Ad Accounts
- **get_ad_analytics**: Requires pivot and dateRange parameters.

Query performance metrics (impressions, clicks, spend)
- **list_campaign_groups**: List campaign groups for an ad account
- **list_ad_campaigns**: List all campaigns for an ad account
- **list_conversion_rules**: List conversion tracking rules for an account
- **list_ad_creatives**: List all ad creatives for an ad account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my LinkedIn Ad accounts."

**🤖 AI Agent:**
> I've retrieved your ad accounts. You have 2 active accounts: 'Global Marketing (ID: 500123)' and 'Retargeting EMEA (ID: 500456)'.

---

**👤 You:**
> "Show performance metrics for account ID '500123' for the year 2024."

**🤖 AI Agent:**
> I've queried the analytics. For the year 2024, account 500123 has generated 1,500,000 impressions and 45,000 clicks, with a total spend of $12,500.00.

---

**👤 You:**
> "List all campaigns associated with my account."

**🤖 AI Agent:**
> I found 5 campaigns in your account, including 'Brand Awareness Q1', 'Lead Gen Webinar', and 'Product Demo'. Which one would you like to see demographics for?


## ❓ FAQ

**Q: Which scopes are required for this server?**
Your access token must have at least `r_ads_reporting` and `r_ads` scopes to list accounts and fetch performance metrics.

**Q: How do I specify the time range for analytics?**
You must provide a Restli-formatted string in the `params` field, including `dateRange=(start:(day:X,month:Y,year:Z))`. Refer to LinkedIn API documentation for exact syntax.

**Q: Is the API Key (Personal Access Token) supported?**
LinkedIn uses OAuth2 tokens. You can generate a long-lived Access Token through the LinkedIn Developer Portal's Token Generator tool for development use.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-ads](https://vinkius.com/mcp/linkedin-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-ads": {
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
