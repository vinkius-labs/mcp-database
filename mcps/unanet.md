# Unanet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unanet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Project-based ERP for government contractors and professional services.

## Description
The Unanet MCP Server connects AI agents to the Unanet project management and ERP suite. It enables agents to read timesheets, view expense reports, query project statuses, and list organizational workforce data, streamlining compliance and operational efficiency.


## Available Tools (4)
- **expenses**: List expense reports for a user
- **projects**: List projects in Unanet
- **timesheets**: List timesheets for a user
- **users**: List users/employees in Unanet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unanet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the submitted expense reports for Project X."

**🤖 AI Agent:**
> There are 4 active expense reports for Project X totaling $1,250.30.

---

**👤 You:**
> "List all pending timesheets for the engineering department this week."

**🤖 AI Agent:**
> Querying Unanet timesheets ('get_timesheets')...
Found 3 pending timesheets for Engineering (Oct 18-24):
1. Alice Baker: 38 hrs (Awaiting Mgr Approval)
2. Charlie P.: 40 hrs (Draft)
3. Dave R.: 32 hrs (Draft)

---

**👤 You:**
> "Check the current compliance status and budget utilization for the 'Alpha-1' defense contract."

**🤖 AI Agent:**
> Analyzing project records ('get_project_details')...
Contract 'Alpha-1' (ID: DEF-771):
- Compliance: DCAA compliant tracking active, 100% compliant.
- Budget: $250,000
- Utilized: $145,200 (58%)
- Status: On Track.


## ❓ FAQ

**Q: What info can the AI query in Unanet?**
It can retrieve project lists and details, expenses, workforce items, and timesheets.

**Q: How do I authenticate this integration?**
Access relies on Basic Authentication. You will need a base environment URL, an integration user's username, and a password/token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unanet](https://vinkius.com/mcp/unanet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unanet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unanet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unanet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unanet": {
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
