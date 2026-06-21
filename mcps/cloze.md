# Cloze MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloze)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Smart CRM that automatically tracks your interactions and provides AI-powered insights.

## Description
Cloze is a smart CRM that automatically tracks your interactions and provides AI-powered insights to manage your relationships, projects, and deals. Through this MCP server, your AI agent can effortlessly pull contact histories, lookup custom tags, verify relationship strengths, and update ongoing project states without breaking your workflow.


## Available Tools
- **create_person**: Provide at least name or email.

Create a new person in Cloze
- **create_project**: Create a new project, deal, or property in Cloze
- **get_person**: Retrieve detailed information about a specific person by email
- **list_companies**: Retrieve a list of companies from Cloze
- **list_custom_fields**: Retrieve definitions for custom fields in your Cloze account
- **list_people**: Retrieve a list of people (contacts) from Cloze
- **list_projects**: Retrieve a list of projects, properties, or deals from Cloze
- **search_people_by_tag**: Find contacts that have a specific tag
- **update_person**: Email is used as the match key.

Update an existing person in Cloze (matching by email)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get all details for the person with email 'sarah@example.com' in Cloze."

**🤖 AI Agent:**
> Contact found: Sarah Johnson (sarah@example.com). Company: TechStart Inc. Stage: Active Lead. Last interaction: March 20, 2025. Score: 85/100. Tags: VIP, Enterprise. Open deals: 2 ($45,000 total pipeline).

---

**👤 You:**
> "Show me my active projects in Cloze."

**🤖 AI Agent:**
> You have 5 active projects:
1. Website Redesign — Due: April 15 (3 tasks remaining)
2. Q2 Marketing Campaign — Due: May 1 (7 tasks)
3. CRM Migration — Due: April 30 (12 tasks)
4. Sales Training — Due: April 10 (1 task)
5. Product Launch — Due: June 1 (15 tasks)

---

**👤 You:**
> "Find all contacts tagged with 'VIP' in Cloze."

**🤖 AI Agent:**
> Found 8 contacts tagged 'VIP':
1. Sarah Johnson — TechStart Inc. (Score: 85)
2. David Chen — FinServe Ltd. (Score: 92)
3. Maria Garcia — CloudFirst (Score: 78)
... Showing 3 of 8. Combined pipeline value: $320,000.


## ❓ FAQ

**Q: Where do I find my Cloze API key?**
You can generate an API key in the Cloze web app. Go to Settings > Accounts and Services, and click the 'API Key' section to add a new token.

**Q: Which email address should I use for authentication?**
Use the exact primary email address registered to your active Cloze account.

**Q: Can I manage custom fields with this server?**
Yes, you can retrieve custom field definitions and command the agent to set specific values when creating or updating contacts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloze](https://vinkius.com/mcp/cloze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloze** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cloze` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloze** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloze": {
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
