# Actionstep MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/actionstep)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Run your law practice smarter with case management, document tracking, and client billing all connected to your AI workflow.

## Description
Connect your **Actionstep** account to any AI agent and simplify your legal operations and workflow management through natural conversation.

### What you can do

- **Matter Management** — List all legal matters, retrieve detailed status metadata, and query historical file notes
- **Contact Tracking** — Query your database of clients, partners, and participants registered in your legal ecosystem
- **Workflow Automation** — List active tasks and matter types to stay on top of your firm's operational pipeline
- **Productivity Insights** — Access billable time entries to understand workload and efficiency
- **Client Control** — Create new contact records programmatically to build your firm's database

### How it works

1. Subscribe to this server
2. Enter your Actionstep OAuth 2.0 Access Token from your developer portal
3. Start managing your legal practice from Claude, Cursor, or any MCP-compatible client


## Available Tools (8)
- **get_matter_details**: Get details for a specific matter
- **list_contacts**: List Actionstep contacts
- **list_matters**: List Actionstep matters
- **list_matter_notes**: List file notes for a matter
- **list_legal_tasks**: List legal workflow tasks
- **list_time_entries**: List billable time entries
- **list_action_types**: List available matter types
- **create_contact**: Register a new contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Actionstep** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active matters in Actionstep."

**🤖 AI Agent:**
> I've fetched your matters. You have 15 active cases, including 'Purchase of 123 Main St' and 'Estate Planning - Miller'.

---

**👤 You:**
> "Find contact details for 'John Smith'."

**🤖 AI Agent:**
> Found John Smith. Email: john@smith.com, Phone: 555-0192. He is associated with 2 active matters.

---

**👤 You:**
> "Show my tasks for today."

**🤖 AI Agent:**
> You have 3 tasks due today: 'Review draft contract', 'Client call at 2 PM', and 'File court documents'.


## ❓ FAQ

**Q: Can I list all my active legal matters using my AI agent?**
Yes! Use the `list_matters` tool to retrieve a comprehensive list of all legal matters registered in your Actionstep system.

**Q: How do I check details for a specific matter?**
Simply provide the Matter ID to the `get_matter_details` tool. Your agent will fetch the full metadata, status, and assigned team.

**Q: Does it support OAuth 2.0 authentication?**
Yes, it uses OAuth 2.0. You'll need to generate a Client ID and Client Secret in your developer portal to create an access token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/actionstep](https://vinkius.com/mcp/actionstep)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Actionstep** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `actionstep` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Actionstep** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "actionstep": {
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
