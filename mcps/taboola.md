# Taboola MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taboola)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage Taboola advertising campaigns, ads, and performance reports directly from any AI agent.

## Description
Connect your **Taboola Backstage** account to any AI agent and take full control of your native advertising workflows through natural conversation.

### What you can do

- **Account Management** — List all allowed accounts and retrieve current user profile details
- **Campaign Control** — List, fetch, create, and update campaigns including budgets, CPC, and active status
- **Ad Management** — Manage campaign items (ads) by listing existing creatives or adding new URLs and thumbnails
- **Performance Reporting** — Run detailed campaign summary reports by dimension (day, week, month) or identify top-performing content

### How it works

1. Subscribe to this server
2. Enter your Taboola Client ID and Client Secret
3. Start optimizing your native ads from Claude, Cursor, or any MCP-compatible client

No more jumping between tabs to check CTR or adjust daily caps. Your AI acts as a dedicated Ad Ops specialist.

### Who is this for?

- **Digital Marketers** — instantly retrieve performance metrics and adjust campaign settings without opening Backstage
- **Ad Ops Teams** — automate the creation of campaign items and monitor account access across multiple clients
- **Growth Engineers** — integrate real-time ad performance data into development workflows for faster iteration


## Available Tools (10)
- **list_allowed_accounts**: List allowed Taboola accounts
- **list_campaign_items**: List items (ads) in a campaign
- **create_campaign**: Create a new Taboola campaign
- **get_current_user**: Get current Taboola user details
- **get_campaign**: Get details for a specific campaign
- **get_top_campaign_content_report**: Get top campaign content report
- **update_campaign**: Update an existing Taboola campaign
- **get_campaign_summary_report**: Get campaign summary report
- **list_campaigns**: List campaigns for an account
- **create_campaign_item**: Create a new campaign item (ad)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taboola** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Taboola accounts."

**🤖 AI Agent:**
> I've retrieved your accounts. You have access to: 'Global_Marketing_US' (ID: act-9821) and 'EMEA_Expansion' (ID: act-4432). Which one would you like to manage?

---

**👤 You:**
> "Get a summary report for account 'act-9821' grouped by day."

**🤖 AI Agent:**
> Fetching the daily summary for 'act-9821'... For the last period, you had 1.2M impressions, 4.5k clicks (0.37% CTR), and a total spend of $2,140. Would you like to see the top-performing items for this account?

---

**👤 You:**
> "Update campaign 'camp-556' in account 'act-9821' to change the CPC to '0.45'."

**🤖 AI Agent:**
> Updating campaign settings... The CPC for 'camp-556' has been successfully updated to 0.45. The campaign remains active with its current daily cap.


## ❓ FAQ

**Q: Can I see how my campaigns are performing across different time periods?**
Yes! Use the `get_campaign_summary_report` tool. You can specify the `account_id` and a `dimension` (like day, week, or month) to get a detailed breakdown of metrics like clicks, impressions, and spend.

**Q: How do I add a new ad to an existing campaign?**
Simply use the `create_campaign_item` action. Provide the `account_id`, `campaign_id`, and the `url` of the content you want to promote. You can also optionally include a custom title and thumbnail URL.

**Q: Is it possible to pause or update the budget of a campaign?**
Yes. The `update_campaign` tool allows you to modify the `daily_cap`, `cpc`, and the `is_active` status of any campaign by providing its ID and the target account ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taboola](https://vinkius.com/mcp/taboola)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Taboola** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `taboola` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Taboola** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taboola": {
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
