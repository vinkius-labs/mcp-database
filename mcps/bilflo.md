# Bilflo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bilflo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage your staffing operations via Bilflo — list clients, contractors, and timecards directly from any AI agent.

## Description
Connect your **Bilflo** account to any AI agent and orchestrate your staffing, recruiting, and time-tracking workflows through natural conversation.

### What you can do

- **Client Management** — List and inspect client profiles to maintain strong business relationships.
- **Contractor Oversight** — Retrieve detailed records for contractors and contingent workers.
- **Placement Tracking** — List both temporary placements and direct hires within your agency.
- **Time & Attendance** — Access timecards and verify hours worked directly from the agent.
- **Compliance & Rules** — Retrieve overtime rules and system configurations for auditing.

### How it works

1. Subscribe to this server
2. Enter your Bilflo API Key
3. Start managing your staffing operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Staffing Agency Managers** — quickly check placement statuses and client details without opening the Bilflo dashboard.
- **Payroll & Billing Teams** — retrieve approved timecards and overtime rules for processing.
- **Recruiters** — verify contractor data and direct hire histories using natural language.


## Available Tools
- **get_client**: Get specific client details
- **get_contractor**: Get specific contractor details
- **get_direct_hire**: Get specific direct hire details
- **get_timecard**: Get specific timecard details
- **list_clients**: List all clients
- **list_contractors**: List all contractors
- **list_direct_hires**: List all direct hires
- **list_overtime_rules**: List overtime rules
- **list_placements**: List all placements
- **list_timecards**: List all timecards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bilflo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active clients in Bilflo."

**🤖 AI Agent:**
> I've retrieved your clients. You have 3 active clients: 'Acme Corp' (ID: cli_1), 'Tech Innovations' (ID: cli_2), and 'Global Solutions' (ID: cli_3).

---

**👤 You:**
> "Find the details for contractor con_992."

**🤖 AI Agent:**
> Contractor 'John Smith' (ID: con_992) is currently on an active placement with 'Acme Corp'. Their next timesheet is due on Friday.

---

**👤 You:**
> "Show my recent timecards."

**🤖 AI Agent:**
> Retrieving timecards... I found 5 recent timecards. 3 are 'Approved' and ready for payroll, and 2 are still in 'Submitted' status awaiting manager approval.


## ❓ FAQ

**Q: Can I check the status of a specific timecard using the agent?**
Yes! Use the `get_timecard` tool with the Timecard ID. Your agent will fetch the latest status, including hours worked and approval state.

**Q: How do I list all the active contractors in Bilflo?**
Simply ask the agent to `list_contractors`. It will retrieve the directory of all contingent workers registered in your Bilflo account.

**Q: Does the integration allow me to approve timecards directly?**
Currently, the toolset is focused on querying and auditing (listing timecards, checking statuses). Approving timecards for payroll must be performed within the Bilflo platform for compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bilflo](https://vinkius.com/mcp/bilflo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bilflo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bilflo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bilflo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bilflo": {
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
