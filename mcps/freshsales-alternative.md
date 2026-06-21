# Freshsales MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshsales-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Close deals faster with AI-powered lead scoring, visual deal pipelines, and built-in phone and email in one sales CRM.

## Description
Connect your **Freshsales** (Freshworks CRM) account to any AI agent and take full control of your sales pipeline and customer relationship workflows through natural conversation.

### What you can do

- **Lead Orchestration** — List and manage new leads programmatically, including retrieving detailed metadata and performing search lookups
- **Pipeline Intelligence** — Monitor sales deals and their current pipeline stages to track revenue and deal velocity in real-time
- **Relationship Management** — Access complete profiles for contacts and sales accounts (companies) to maintain a high-fidelity customer database
- **Task & Activity Tracking** — Monitor pending tasks, appointments, and meetings directly through your agent to coordinate team efforts
- **Note Retrieval** — Access and retrieve contextual notes associated with any CRM record to provide your agent with the latest background info

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Freshsales (Settings > API Settings)
3. Identify your **Account Subdomain** (e.g., 'acme' from acme.freshsales.io)
4. Start managing your sales CRM from Claude, Cursor, or any MCP client

No more manual deal logging or digging through CRM menus. Your AI acts as your dedicated sales operations assistant.

### Who is this for?

- **Sales Teams** — instantly retrieve lead details and update deal stages using natural language commands
- **Account Managers** — monitor recent activities and retrieve customer notes without leaving your workspace
- **Sales Ops Leads** — automate lead creation and monitor pipeline health through simple AI queries


## Available Tools (10)
- **create_lead**: Requires last_name and optionally email.

Create a new lead
- **get_contact**: Get details for a specific contact
- **get_lead**: Get details for a specific lead
- **list_sales_accounts**: List all sales accounts (companies)
- **list_appointments**: List scheduled appointments
- **list_contacts**: List all Freshsales contacts
- **list_deals**: List all sales deals
- **list_leads**: List all Freshsales leads
- **list_notes**: List CRM notes
- **list_tasks**: List CRM tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshsales** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my new leads in Freshsales."

**🤖 AI Agent:**
> I've retrieved your leads. You have 5 new entries, including 'John Doe' (ID: 101) and 'Sarah Smith' (ID: 102). Would you like to check the metadata for any of them?

---

**👤 You:**
> "Show me the last 5 sales deals and their stages."

**🤖 AI Agent:**
> Scanning deals... Here are the last 5: 'Cloud Migration' (Negotiation), 'License Renewal' (Closed Won), and 3 others. Shall I provide the deal value for the active ones?

---

**👤 You:**
> "Get details for contact ID '12345'."

**🤖 AI Agent:**
> Fetching contact 12345... This profile is for 'Mike Ross'. He is associated with 'Pearson Specter' and has 2 pending tasks. Would you like to read the latest notes for this contact?


## ❓ FAQ

**Q: How do I find my Freshsales API Key?**
Log in to Freshsales, click on your profile icon (top right), go to **Settings** > **API Settings**, and copy your unique key.

**Q: Can I search for leads by email?**
The `list_leads` tool retrieves the directory of leads. You can ask your agent to filter or find specific records by email within the returned data.

**Q: Does it support listing individual sales accounts?**
Yes! Use the `list_sales_accounts` tool to retrieve a comprehensive list of all company/account records in your Freshsales CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshsales-alternative](https://vinkius.com/mcp/freshsales-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `freshsales-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshsales** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshsales-alternative": {
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
