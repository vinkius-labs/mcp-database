# Zoho CRM Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage marketing campaigns, track campaign leads and contacts — full marketing automation in Zoho CRM.

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools (6)
- **zoho_campaign_contacts**: Returns contacts with name, email, account, and status. Use to see which qualified contacts (converted leads or existing customers) are part of a campaign, for engagement analysis, or re-targeting decisions.

Get all contacts associated with a specific campaign to measure conversion and engagement at the customer level
- **zoho_campaign_leads**: Returns leads with name, email, company, and source. Use to measure campaign effectiveness: "how many leads did this campaign generate?", "which leads came from the webinar?", or for campaign ROI analysis.

Get all leads associated with a specific campaign to measure lead generation performance and attribution
- **zoho_create_campaign**: Campaign_Name is required. Type: Conference, Webinar, Trade Show, Public Relations, Advertisement, Email, Social Media, Banner Ads. Status: Planning, Active, Inactive, Complete, None. Start_Date/End_Date use YYYY-MM-DD. Budgeted_Cost is the planned spend.

Create a new marketing campaign in Zoho CRM with name, type, budget, dates, and status for initiative tracking
- **zoho_get_campaign**: Returns full data: name, type, status, budgeted/actual cost, expected revenue, expected response, start/end dates, and description. Use after searching to drill into campaign details.

Get complete details of a specific Zoho CRM campaign by ID, including budget, ROI metrics, and all custom fields
- **zoho_list_campaigns**: Returns campaign name, type, status (Planning/Active/Inactive/Complete), budgeted and actual costs, start/end dates, and expected response rates. Use when the user asks about marketing initiatives, campaign budgets, or active promotions.

List marketing campaigns in Zoho CRM with name, type (Conference/Webinar/Email/Advertisement), status, budget, and dates
- **zoho_search_campaigns**: Returns matching campaigns with type, status, budget, and dates. Use when the user wants to find a specific campaign, check its budget/ROI, or review campaign status.

Search Zoho CRM campaigns by name or keyword to find specific marketing initiatives and their performance data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from web form"

**🤖 AI Agent:**
> 👥 **Leads from Web Form**
| Name | Email | Company | Status |
|---|---|---|---|
| John Smith | john@acme.com | Acme Corp | New |
| Maria Garcia | maria@beta.io | Beta Inc | Contacted |

---

**👤 You:**
> "Create a deal: Enterprise Plan $25,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Plan
- Amount: $25,000
- Stage: Qualification
- Closing: 2024-03-30


## ❓ FAQ

**Q: What Zoho CRM data can I access?**
Leads, Contacts, Accounts, Deals, Notes, and any custom module. All data respects your Zoho CRM permissions.

**Q: How does authentication work?**
Uses Zoho OAuth 2.0 with a refresh token. Create a Self Client in the Zoho API Console, generate a refresh token, and provide Client ID, Client Secret, and Refresh Token.

**Q: Does it support multi-region Zoho?**
Yes! Set your API domain: zohoapis.com (US), zohoapis.eu (EU), zohoapis.in (India), zohoapis.com.au (Australia), zohoapis.jp (Japan).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-marketing](https://vinkius.com/mcp/zoho-crm-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho CRM Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-crm-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho CRM Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-crm-marketing": {
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
