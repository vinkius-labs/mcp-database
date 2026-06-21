# Armano MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/armano)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your business systems through intelligent iPaaS integration that syncs data across apps without custom development.

## Description
Connect your **Armano** account to any AI agent and take full control of your human resources and automated workforce orchestration through natural conversation.

### What you can do

- **Workforce Portfolio Orchestration** — List and manage your entire database of employees programmatically, retrieving detailed profiles and department affiliations
- **Time & Attendance Intelligence** — Programmatically retrieve time tracking records and monitor clock-in/out metadata to maintain a perfectly coordinated audit trail
- **Absence & Leave Architecture** — Access your complete directory of time-off requests and statuses to oversee your organizational resource allocation
- **Document Monitoring** — Access real-time status updates for employee records and retrieve hosted assets directly through your agent
- **Operational Monitoring** — Verify account-level API connectivity and monitor HR process volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Armano dashboard (App Integrations section)
3. Start orchestrating your workforce from Claude, Cursor, or any MCP client

No more manual checking of individual employee cards or missing leave requests. Your AI acts as your dedicated HR coordinator and workforce architect.

### Who is this for?

- **HR Managers** — instantly retrieve employee summaries and monitor team attendance using natural language commands
- **Department Leads** — verify individual absence requests and track team availability without leaving your workspace
- **Developers** — integrate high-speed Armano HR data into custom internal tools through simple AI queries


## Available Tools (10)
- **list_employees**: List all employees
- **list_leaves**: List all leave requests
- **list_projects**: List all projects
- **list_time_entries**: Optionally filter by date range (YYYY-MM-DD format).

List time entries
- **check_armano_status**: Verify Armano API connectivity
- **create_time_entry**: Create a time entry
- **get_employee**: Get employee details
- **get_project**: Get project details
- **get_time_entry**: Get time entry details
- **list_departments**: List all departments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Armano** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in my Armano account."

**🤖 AI Agent:**
> I've retrieved your employee directory. You currently have 50 active profiles, including 'John Doe' (Department: Sales) and 'Sarah Manager'. Would you like the detailed role metadata for any of them?

---

**👤 You:**
> "Show the time entries for 'Sarah Manager' from yesterday."

**🤖 AI Agent:**
> Time intelligence orchestrated! For Sarah Manager, I've identified 2 entries from yesterday: Clock-in at 9:00 AM and Clock-out at 5:00 PM. I've retrieved the technical location metadata for your review. Need help auditing the total hours?

---

**👤 You:**
> "Check for any pending absence requests for this week."

**🤖 AI Agent:**
> Absence architecture orchestrated! I've identified 3 pending requests for this week, including 2 days for 'Mike Employee'. I've retrieved the technical request metadata and overlap status for your review. Shall I notify the managers?


## ❓ FAQ

**Q: How do I find my Armano API Key?**
Log in to your account, navigate to **Settings** > **App Integrations**, and copy your unique API Token from the credentials section.

**Q: Can I retrieve time entries via AI?**
Yes! The `list_time_entries` tool allows your agent to retrieve clock-in/out records for any specific period.

**Q: How do I list my active employees?**
Use the `list_employees` tool to retrieve your complete directory along with the unique identifiers for all registered staff members.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/armano](https://vinkius.com/mcp/armano)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Armano** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `armano` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Armano** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "armano": {
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
