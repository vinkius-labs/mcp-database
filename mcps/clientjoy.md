# Clientjoy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientjoy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage agency CRM and invoicing via Clientjoy — track leads, monitor invoices, and manage client projects directly from any AI agent.

## Description
Connect your **Clientjoy** account to any AI agent and take full control of your agency operations through natural conversation. Streamline how you manage the entire lifecycle from lead capture to final invoicing natively.

### What you can do

- **Lead Oversight** — List and retrieve details for all sales leads and their capture status natively
- **Contact Intelligence** — Access and monitor all client contacts and relationship history flawlessly
- **Invoicing Logistics** — List all agency invoices and monitor their payment status flawlessly
- **Project Management** — Access and monitor all client projects and their constituent tasks securely
- **Sales Pipelines** — List and review quotes and proposals sent to potential clients flawlessly
- **Profile Visibility** — Access your own user profile and core workspace metadata directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your Clientjoy API Token (obtained from Settings > API)
3. Start managing your agency CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Owners** — monitor sales pipelines and revenue status using natural language
- **Project Managers** — audit project progress and task lists without opening the dashboard
- **Accountants** — quickly look up invoice status and payment history straight from their chat interface
- **Sales Teams** — verify lead profiles and proposal statuses


## Available Tools (8)
- **get_contact_crm_details**: Get detailed information for a specific contact
- **get_lead_crm_details**: Get detailed information for a specific lead
- **get_my_clientjoy_profile**: Retrieve information about the authenticated workspace user
- **list_clientjoy_contacts**: List all contacts and clients stored in the CRM
- **list_agency_invoices**: List all invoices and their payment status
- **list_clientjoy_leads**: List all sales leads captured in Clientjoy
- **list_agency_projects**: List all client projects tracked in Clientjoy
- **list_sales_quotes**: List sales quotes and proposals sent to clients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clientjoy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my new leads in Clientjoy."

**🤖 AI Agent:**
> Retrieving your leads... I found 5 items: John Doe (Qualified), Jane Smith (New), Mike Scott (Interested), and 2 others. Would you like the details for the new lead?

---

**👤 You:**
> "Show me my unpaid invoices."

**🤖 AI Agent:**
> Checking invoices... You have 3 unpaid invoices: #INV-101 ($1,200), #INV-105 ($450), and #INV-108 ($2,100). The first two are currently overdue.

---

**👤 You:**
> "What is the status of the 'Website Redesign' project?"

**🤖 AI Agent:**
> Checking projects... The 'Website Redesign' project for Acme Corp is 'In Progress'. It has 12 completed tasks and 5 pending items.


## ❓ FAQ

**Q: Can I see which invoices are still unpaid?**
Yes! Use the `list_agency_invoices` tool. The agent will return all invoices, and you can ask it to filter for those with an 'Unpaid' or 'Overdue' status.

**Q: How do I check the status of a specific sales proposal?**
Use the `list_sales_quotes` tool. Your agent will fetch all quotes and proposals, showing their current status (e.g., Sent, Viewed, Accepted).

**Q: Where do I find my Clientjoy API Token?**
Log in to your Clientjoy account, navigate to **Settings**, and select **API**. You can generate and copy your API token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientjoy](https://vinkius.com/mcp/clientjoy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clientjoy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clientjoy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clientjoy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clientjoy": {
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
