# Agile CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agile-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Sales and marketing automation — manage contacts, deals, tasks, and campaigns via AI.

## Description
Connect your **Agile CRM** account to your AI agent to unlock powerful CRM and marketing automation. From creating and managing contact profiles to auditing your sales pipeline and orchestrating task workflows, your agent handles your business interactions through natural conversation.

### What you can do

- **Unified Contact Management** — Create, update, and search for contacts, including managing custom properties and tags
- **Pipeline Orchestration** — List and audit sales deals, check pipeline stages, and retrieve technical metadata for opportunities
- **Task & Activity Tracking** — List and create tasks to ensure your team stays on top of follow-ups and client meetings
- **Account Intelligence** — Search for contacts by email and retrieve historical interaction logs to support sales outreach
- **Workflow Monitoring** — Quickly identify high-value deals or overdue tasks directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Agile CRM Domain, Email, and REST API Key
3. Start managing your CRM and monitoring your sales pipeline through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — research prospects and update deal statuses without leaving the chat
- **Marketing Managers** — audit contact lists and manage segment tags effortlessly
- **Customer Success** — look up client history and create follow-up tasks using simple commands
- **Business Owners** — retrieve sales performance summaries and identify bottlenecks in the pipeline


## Available Tools
- **list_contacts**: List CRM contacts
- **search_contact_by_email**: Search contact by email
- **list_deals**: List sales opportunities
- **list_tasks**: List CRM tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agile CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 contacts created in Agile CRM."

**🤖 AI Agent:**
> I've retrieved the latest 5 contacts. They include John Smith, Maria Garcia, and 3 others. Would you like to see the active deals for any of these contacts?

---

**👤 You:**
> "Show me all deals worth more than $5,000."

**🤖 AI Agent:**
> I've filtered your pipeline. You have 4 deals with values over $5,000, including 'Enterprise Software License' and 'Premium Support Plan'. Total potential revenue from these is $32,000.

---

**👤 You:**
> "Search for contact 'jane.doe@example.com' and show recent tasks."

**🤖 AI Agent:**
> I've found Jane Doe. She has 2 pending tasks: 'Send Proposal' (due today) and 'Follow-up Call' (due Friday). Would you like to mark any of these as completed?


## ❓ FAQ

**Q: How do I find my Agile CRM REST API Key?**
Log in to Agile CRM, go to **Admin Settings** > **Developers & API**. You will find your REST API Key listed there. Use this along with your account email for authentication.

**Q: Can I search for a contact by email?**
Yes! Use the `search_contact_by_email` tool. It provides a direct way to find a contact profile using their email address, returning their full history and properties.

**Q: Does this support custom properties?**
Yes, custom properties are included in the contact details retrieved via the API. You can also update them by specifying the property name and value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agile-crm](https://vinkius.com/mcp/agile-crm)
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
3. Set Type to "SSE", enter `agile-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agile CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agile-crm": {
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
