# Agile CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agile-crm-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage contacts, deals, and marketing campaigns in one place with a CRM built for growing sales teams.

## Description
Connect your **Agile CRM** account to any AI agent and take full control of your sales, marketing, and service automation workflows through natural conversation.

### What you can do

- **Contact & Relationship Orchestration** — List and manage your entire high-fidelity contact directory programmatically, retrieving detailed profile metadata and interaction notes
- **Deal Lifecycle Management** — Monitor your sales pipeline in real-time, create new high-fidelity opportunities, and track deal probability and values directly through your agent
- **Task & Event Intelligence** — Programmatically organize your daily workflow by creating tasks and calendar events to maintain a perfectly coordinated team schedule
- **Customer Discovery** — Access complete profile properties including custom tags and high-fidelity contact history to oversee your organizational relationship ecosystem
- **Operational Monitoring** — Access account-level configuration and verify API connectivity directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key**, **Email**, and **Domain** from your Agile CRM dashboard (Admin Settings > Developers & API)
3. Start orchestrating your business growth from Claude, Cursor, or any MCP client

No more manual status checking across different CRM modules or digging through complex deal tables. Your AI acts as your dedicated sales coordinator and relationship architect.

### Who is this for?

- **Sales Executives** — instantly retrieve deal summaries and update contact records using natural language commands
- **Marketing Teams** — monitor lead distribution and task priorities without leaving your workspace
- **Operations Leads** — automate the oversight of sales pipelines and team calendars through simple AI queries


## Available Tools (12)
- **create_deal**: Create a new deal
- **delete_contact**: Delete a contact
- **list_contacts**: List all contacts in Agile CRM
- **list_deals**: List all deals (opportunities)
- **list_events**: List all calendar events
- **list_contact_notes**: List notes for a specific contact
- **list_tasks**: List all tasks
- **retrieve_contact**: Get details of a specific contact
- **retrieve_deal**: Get details of a specific deal
- **retrieve_task**: Get details of a specific task
- **update_contact**: Update an existing contact
- **create_contact**: Create a new contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agile CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sales deals in my Agile CRM pipeline."

**🤖 AI Agent:**
> I've retrieved your active deals. You currently have 10 opportunities in the pipeline, including 'Web Redesign' (Value: $5,000) and 'Enterprise License'. Would you like the detailed probability metadata for any of these?

---

**👤 You:**
> "Create a new contact 'John Doe' (john@example.com) and add a note about our last meeting."

**🤖 AI Agent:**
> Contact orchestrated! I've successfully created the profile for John Doe (ID: cont_123) and registered your high-fidelity meeting note in his profile. He is now active in your CRM. Need help creating a follow-up task?

---

**👤 You:**
> "What are my pending tasks and events for today?"

**🤖 AI Agent:**
> Accessing schedule... Today you have 3 pending tasks, including 'Call Acme Corp', and a 'Project Sync' event at 2 PM. I've retrieved the high-fidelity due times for your organizational alignment. Need more historical context?


## ❓ FAQ

**Q: How do I find my Agile CRM API Key?**
Log in to your dashboard, navigate to **Admin Settings** > **Developers & API**, and copy your REST API Key.

**Q: Can I create new deals via AI?**
Yes! The `create_deal` tool allows your agent to register new sales opportunities by providing deal name, value, and probability programmatically.

**Q: How do I find my Agile CRM domain?**
Your domain is the prefix of your Agile CRM URL. For example, if you log in at `vinkius.agilecrm.com`, your domain is `vinkius`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agile-crm-alternative](https://vinkius.com/mcp/agile-crm-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agile CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agile-crm-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agile CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agile-crm-alternative": {
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
