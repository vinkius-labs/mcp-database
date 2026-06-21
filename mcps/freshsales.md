# Freshsales MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshsales)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage your CRM pipelines, track leads, and oversee sales deals via AI agents with Freshsales.

## Description
Connect your **Freshsales** account to any AI agent to automate your sales CRM operations through the Model Context Protocol (MCP). Freshsales is a powerful sales CRM that provides a 360-degree view of your customers. This MCP server enables you to track active deals, manage lead data, and retrieve detailed contact profiles directly through natural conversation.

### Key Features

- **Lead & Contact Oversight** — List all leads and contacts, fetch detailed profiles, and create new leads instantly to keep your pipeline full.
- **Deal Management** — Access your sales opportunities, monitor deal stages, and retrieve detailed metadata to track revenue.
- **Account Discovery** — List and search for company accounts to maintain full context of your B2B relationships.
- **Task & Appointment Tracking** — Monitor scheduled meetings and pending sales tasks to ensure no follow-up is missed.
- **Sales Team Insights** — List all CRM users and sales representatives to understand territory assignments and workloads.
- **Real-time Synchronization** — Keep your sales data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshsales Domain prefix and API Token (found in your Profile Settings)
3. Start managing your CRM data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Managers** — quickly check deal stages or sales rep workloads without manual dashboard navigation.
- **Account Executives** — get a real-time overview of lead profiles and scheduled appointments via simple AI commands.
- **SDRs & BDRs** — automate the creation of new leads and verify contact details seamlessly.


## Available Tools (12)
- **create_crm_lead**: Create a new lead
- **get_account_details**: Get account metadata
- **get_contact_metadata**: Get contact details
- **get_deal_details**: Get deal metadata
- **get_lead_details**: Get lead metadata
- **list_sales_accounts**: List CRM accounts
- **list_appointments**: List scheduled appointments
- **list_crm_contacts**: List CRM contacts
- **list_crm_deals**: List sales deals
- **list_crm_leads**: List CRM leads
- **list_crm_tasks**: List pending tasks
- **list_crm_users**: List CRM users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshsales** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent active sales deals."

**🤖 AI Agent:**
> Retrieving deals... I found 5 active opportunities, including 'Acme Corp Software Expansion' ($50,000) and 'Globex Renewal' ($15,000). Would you like to see their current stages?

---

**👤 You:**
> "Show me the contact details for 'Jane Smith'."

**🤖 AI Agent:**
> Searching contacts... I found Jane Smith (jane@example.com). She is the VP of Sales at Example Inc. and has 2 active deals associated with her profile.

---

**👤 You:**
> "Create a new lead for 'John Doe' (johndoe@email.com)."

**🤖 AI Agent:**
> Lead created! I have successfully added 'John Doe' (johndoe@email.com) to your CRM. The new Lead ID is 98765.


## ❓ FAQ

**Q: How do I get an API Key for Freshsales?**
Log in to your Freshsales account, click on your Profile picture in the top-right corner, go to 'Profile Settings', and navigate to the 'API Settings' tab to find your Token.

**Q: What is my 'Domain prefix'?**
Your domain prefix is the first part of your Freshsales or Freshworks CRM URL (e.g. if your URL is 'acme.myfreshworks.com/crm/sales' or 'acme.freshsales.io', the prefix is 'acme').

**Q: Can I create a new lead through the agent?**
Yes! Use the 'create_crm_lead' tool and provide the first name, last name, and optionally an email address to instantly add them to your CRM.

**Q: Are custom fields supported?**
When you retrieve a record (like a deal or contact) using tools like 'get_deal_details', the agent fetches the complete metadata payload, which includes all configured custom fields.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshsales](https://vinkius.com/mcp/freshsales)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freshsales** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freshsales` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshsales** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshsales": {
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
