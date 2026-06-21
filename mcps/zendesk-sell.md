# Zendesk Sell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zendesk-sell)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage sales leads, contacts, and deals via the Zendesk Sell (Base CRM) API.

## Description
Connect your **Zendesk Sell** (formerly Base CRM) account to any AI agent to automate your sales pipeline and customer management. This MCP server enables your agent to interact with leads, qualified contacts, and sales deals directly from natural language interfaces.

### What you can do

- **Lead Management** — List, retrieve, and create sales leads to capture potential customer interest
- **Contact Oversight** — Manage qualified people and organizations, and retrieve their complete metadata profiles
- **Deal Tracking** — Monitor sales opportunities, update their status, and manage the entire deal lifecycle
- **Pipeline Automation** — Create and update sales records directly from your conversation to keep your CRM accurate
- **CRM Cleanup** — Delete unnecessary leads, contacts, or deals via simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your Zendesk Sell Personal Access Token
3. Start managing your sales CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — Quickly update deal statuses and lead notes without logging into the dashboard
- **Sales Managers** — Monitor pipeline health and track team opportunities via natural language commands
- **Operations Teams** — Automate the creation of sales records and maintain database hygiene effortlessly


## Available Tools (11)
- **list_sales_contacts**: List all sales contacts (qualified prospects)
- **create_sales_contact**: Requires a JSON body with contact details.

Create a new person or organization contact
- **create_sales_deal**: Requires deal name and contact_id.

Create a new sales opportunity (deal)
- **create_new_lead**: Requires last_name or organization_name.

Create a new sales lead
- **list_sales_deals**: List all sales deals (opportunities)
- **delete_sales_deal**: Remove a deal from the account
- **get_sales_contact_details**: Get details for a specific contact
- **get_deal_details**: Get details for a specific sales deal
- **get_lead_details**: Get details for a specific lead
- **list_sales_leads**: List all sales leads
- **update_existing_deal**: Update details for an existing deal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zendesk Sell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sales leads in my Zendesk Sell account."

**🤖 AI Agent:**
> I've retrieved your leads. You have 15 active leads, including 'John Smith' from 'Acme Corp' and 'Jane Doe' from 'Global Tech'. Would you like to see more details for any of them?

---

**👤 You:**
> "Create a new deal named 'Enterprise License' for contact ID '98765'."

**🤖 AI Agent:**
> Successfully created the deal 'Enterprise License' for contact 98765. The new deal ID is '54321' and its initial status is 'Incoming'.

---

**👤 You:**
> "Update the status of deal '54321' to 'Won'."

**🤖 AI Agent:**
> Successfully updated deal 54321. The status is now marked as 'Won' in your Zendesk Sell pipeline. Congratulations!


## ❓ FAQ

**Q: What is the difference between a Lead and a Contact in Zendesk Sell?**
Leads represent potential interest but are not yet qualified. Contacts are qualified individuals or organizations that can be associated with sales deals.

**Q: Can I associate a deal with a contact via the agent?**
Yes, when using the `create_sales_deal` tool, you must provide a `contact_id` to link the new opportunity to an existing person or company.

**Q: How do I update the status of an existing deal?**
Use the `update_existing_deal` tool with the unique deal ID and a JSON object containing the new status (e.g., 'Won', 'Lost', or a specific pipeline stage).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zendesk-sell](https://vinkius.com/mcp/zendesk-sell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zendesk Sell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zendesk-sell` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zendesk Sell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zendesk-sell": {
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
