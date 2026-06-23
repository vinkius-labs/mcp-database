# Salesforce Marketing Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-marketing-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage campaigns, track member engagement, measure marketing ROI, and optimize lead generation through natural conversation.

## Description
Connect **Salesforce Marketing** to any AI agent.

### What you can do
- **Campaigns** — Search, create, and filter by status
- **Members** — View and add leads/contacts to campaigns
- **Performance** — Aggregate metrics by campaign type

### Who is this for?
- **Marketing Managers** — Campaign health at a glance
- **Demand Gen** — Track lead-to-conversion by campaign
- **Growth Teams** — ROI analysis through conversation


## Available Tools (6)
- **sf_add_campaign_member**: Provide campaignId and either contactId OR leadId (not both). Status defaults to "Sent" but can be set to "Responded", "Registered", etc. based on your campaign member statuses. Returns the created membership record.

Add a lead or contact to a Salesforce marketing campaign for attribution tracking and engagement measurement
- **sf_create_campaign**: Name is required. Type: Email, Conference, Webinar, Trade Show, Public Relations, Advertisement, Banner Ads, Telemarketing. Status defaults to "Planned". Dates use YYYY-MM-DD. budgetedCost is the planned spend. Returns the created campaign with its Salesforce ID.

Create a new marketing campaign in Salesforce with name, type, status, dates, description, and budget
- **sf_campaign_members**: Returns member name, type (Lead or Contact), status (Sent/Responded/etc.), and response date. Use to see who is in a campaign, track engagement, or analyze campaign reach. Essential for campaign ROI and attribution analysis.

Get all leads and contacts enrolled in a specific Salesforce campaign with their membership status and response dates
- **sf_campaign_performance**: Returns the number of campaigns, total leads generated, total conversions, total budgeted cost, and actual cost per campaign type. Provides an instant ROI overview across all marketing channels. Use for marketing dashboard, channel-level performance comparison, or budget allocation analysis.

Get aggregate marketing campaign performance — campaign counts, total leads, conversions, and costs grouped by campaign type
- **sf_campaigns_by_status**: Returns campaigns with lead/contact counts, budget, and conversion data. Use for questions like "which campaigns are currently running?" or "show completed campaigns with their results."

Get Salesforce campaigns filtered by status — Planned, In Progress, Completed, or Aborted — with full metrics
- **sf_search_campaigns**: Returns campaign name, status (Planned/In Progress/Completed/Aborted), type (Email/Conference/Webinar/Advertisement), start/end dates, number of leads generated, contacts converted, budgeted cost, and actual cost. Use when the user asks about marketing initiatives, campaign performance, or budget spend.

Search Salesforce marketing campaigns by name to find initiatives with status, type, budget, and lead/contact conversion metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Marketing Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the conversion rate of our Email campaigns?"

**🤖 AI Agent:**
> 📧 **Email Campaign Performance**
- 5 active campaigns
- 1,200 total leads
- 340 conversions (28.3%)
- Total cost: $12,500

---

**👤 You:**
> "Create a new webinar campaign for Q2 product launch"

**🤖 AI Agent:**
> ✅ **Campaign Created!**
- Name: Q2 Product Launch Webinar
- Type: Webinar
- Status: Planned
- Budget: $5,000

---

**👤 You:**
> "Show me all in-progress campaigns"

**🤖 AI Agent:**
> 🎯 **In Progress Campaigns**
| Name | Leads | Converted | Budget |
|---|---|---|---|
| Spring Webinar | 450 | 89 | $3,000 |
| LinkedIn Ads Q1 | 1,200 | 234 | $15,000 |


## ❓ FAQ

**Q: What campaign data can I access?**
Search campaigns, view members, track conversions, measure costs and ROI — all grouped by type.

**Q: Can I add leads to campaigns?**
Yes! Add any Lead or Contact as a campaign member with a specific status.

**Q: How is campaign performance measured?**
Aggregate metrics: total leads, conversions, actual cost per campaign type. Compare ROI across channels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-marketing-cloud](https://vinkius.com/mcp/salesforce-marketing-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Marketing Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salesforce-marketing-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Marketing Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-marketing-cloud": {
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
