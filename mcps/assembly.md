# Assembly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assembly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage Assembly clients, companies, workspaces, and notes.

## Description
# Assembly

The Assembly MCP Server allows AI agents to interact with your Assembly platform data seamlessly.

### What you can do
- Retrieve clients, companies, and users.
- Access workspaces and CRM details.
- Manage notes and internal data.

### How it works
Connect your Assembly account via your API Key to manage your professional service data dynamically.


## Available Tools (10)
- **get_client**: Get details for a specific client
- **get_company**: Get details for a specific company
- **get_note**: Get a specific note
- **get_user**: Get details for a specific user
- **get_workspace**: Get a specific workspace
- **list_clients**: List all Assembly clients
- **list_companies**: List all Assembly companies
- **list_notes**: List Assembly notes
- **list_users**: List all Assembly users
- **list_workspaces**: List all Assembly workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assembly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all clients in Assembly."

**🤖 AI Agent:**
> I retrieved your clients. Here are the active ones: 'Vinkius', 'Google'.

---

**👤 You:**
> "Get companies in my account."

**🤖 AI Agent:**
> Here are your companies, including 5 active clients.

---

**👤 You:**
> "Show all workspaces and the latest notes created this month."

**🤖 AI Agent:**
> You have 3 active workspaces: 'Consulting Ops' (ws_201, 12 members), 'Product Dev' (ws_202, 8 members), and 'Finance' (ws_203, 4 members). This month you have 7 notes — the most recent are 'Q2 Revenue Forecast' (note_891, updated yesterday), 'Client Onboarding Checklist' (note_888), and 'Sprint Retrospective' (note_885). Would you like to open any of these?


## ❓ FAQ

**Q: Where do I find my API Key?**
Your API Key can be found in your Assembly web portal under Settings > API.

**Q: What access does this MCP need?**
It requires the REST API Key, giving access to clients, companies, users, and notes.

**Q: Can I browse workspaces and internal notes through the AI agent?**
Yes. Use `list_workspaces` to see all workspaces and `get_workspace` to inspect a specific one. For notes, `list_notes` retrieves all entries and `get_note` fetches the full content of a specific note by ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assembly](https://vinkius.com/mcp/assembly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assembly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `assembly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assembly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assembly": {
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
