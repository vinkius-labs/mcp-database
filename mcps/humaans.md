# Humaans MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/humaans)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employees, leaves, and organization data via Humaans HRIS API.

## Description
Connect your AI agents to Humaans, the modern HRIS for global teams. This MCP server allows you to list and manage employees, track leave requests, view public holidays, and access organization data like teams, departments, and offices directly through the Humaans API. Ideal for automating HR operations and employee directory lookups.


## Available Tools (10)
- **get_employee**: Retrieves details for a specific employee
- **get_me**: Gets current authenticated user info
- **list_departments**: Lists organization departments
- **list_documents**: Lists company and employee documents
- **list_employees**: Lists all employees
- **list_leaves**: Lists employee leave requests
- **list_offices**: Lists organization offices
- **list_public_holidays**: Lists public holidays
- **list_roles**: Lists job roles
- **list_teams**: Lists organization teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Humaans** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the London office."

**🤖 AI Agent:**
> I'll fetch the employee list and filter by the London office for you.

---

**👤 You:**
> "Who is currently on leave?"

**🤖 AI Agent:**
> I'll check the current leave requests to see who is away.

---

**👤 You:**
> "Show me the organization chart (teams and departments)."

**🤖 AI Agent:**
> I'll retrieve the list of teams and departments for you.


## ❓ FAQ

**Q: How do I get Humaans API credentials?**
You can generate an Access Token in your Humaans user profile settings under 'API'. Ensure you have the necessary permissions to access organizational data.

**Q: Can I see salary information?**
Access to sensitive fields like salary depends on the permissions of the Access Token provided. This MCP uses the standard people and organization endpoints.

**Q: Does it support leave management?**
Yes, the list_leaves tool allows you to track and monitor employee leave requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/humaans](https://vinkius.com/mcp/humaans)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Humaans** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `humaans` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Humaans** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "humaans": {
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
