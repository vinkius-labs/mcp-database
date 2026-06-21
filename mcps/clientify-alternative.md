# Clientify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientify-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Grow your sales pipeline with a CRM that combines lead capture, email marketing, and deal tracking for Spanish-speaking markets.

## Description
Connect your **Clientify** CRM account to any AI agent and streamline your entire sales process through natural conversation.

### What you can do

- **Contact Management** — List, create, and update contacts with deep inspection of custom fields and social metadata.
- **Sales Pipelines** — Track deals across different stages, update amounts, and assign opportunities to specific pipelines.
- **Task Scheduling** — Create and manage activities like calls, meetings, and follow-ups to never miss a lead.
- **Team Visibility** — List account users and collaborators to understand your organizational structure.
- **Automated Insights** — Fetch real-time summaries of your sales activities and deal progress.

### How it works

1. Subscribe to this server
2. Enter your Clientify API Token (found in your account settings under API)
3. Start managing your sales machine from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Reps** — quickly update deal statuses and log call notes without manual CRM data entry.
- **Marketing Managers** — query contact segments and verify campaign leads directly from your workspace.
- **Business Owners** — get instant bird's-eye views of your sales pipelines and team activity levels.


## Available Tools
- **create_activity**: Create a new activity or task
- **create_contact**: Create a new contact in Clientify
- **create_deal**: Create a new sales deal
- **get_contact**: Get details for a specific contact
- **list_activities**: List all tasks and activities
- **list_contacts**: Supports filtering by email for precise lookups.

List all contacts from Clientify
- **list_deals**: List all deals/opportunities
- **list_pipelines**: List all deal pipelines
- **list_users**: List all account users
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clientify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active deals in the main pipeline."

**🤖 AI Agent:**
> I've retrieved your deals. There are 4 active opportunities including 'Project Alpha' ($5,000) and 'Enterprise License' ($12,000). Both are in the 'Discovery' stage. Would you like more details on any of these?

---

**👤 You:**
> "Create a new contact for John Doe (john@example.com)."

**🤖 AI Agent:**
> Successfully created! John Doe has been added to Clientify with ID 88923. I've also linked his email address john@example.com. Shall I schedule a follow-up call for tomorrow?

---

**👤 You:**
> "List all team members who have access to this account."

**🤖 AI Agent:**
> I've fetched the user directory. There are 3 active users: Sarah (Admin), Mike (Sales), and Elena (Marketing). Let me know if you need to assign a deal to one of them.


## ❓ FAQ

**Q: Can I search for a contact using only their email address?**
Yes. Use the `list_contacts` tool and provide the email in the optional parameter. The agent will return the specific contact record associated with that email if it exists in your CRM.

**Q: How do I move a deal to a different stage in the pipeline?**
You can update deal details using our action tools. Simply specify the Deal ID and the new Pipeline Stage ID to transition the opportunity instantly.

**Q: Does this integration support creating new tasks for follow-ups?**
Absolutely. The `create_activity` tool allows you to schedule calls, meetings, or tasks, assign them to contacts, and set due dates directly from the AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientify-alternative](https://vinkius.com/mcp/clientify-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clientify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clientify-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clientify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clientify-alternative": {
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
