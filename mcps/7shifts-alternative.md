# 7shifts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/7shifts-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedule restaurant staff, manage shifts, track labor costs, and coordinate your team with intelligent workforce planning.

## Description
Connect your **7shifts** restaurant management account to any AI agent and simplify how you coordinate your workforce, manage shift assignments, and track labor costs through natural conversation.

### What you can do
- **Employee Management** — List all staff members, create new employee profiles, and retrieve detailed metadata for individual users.
- **Shift Coordination** — Create, list, and monitor work assignments across different locations and departments.
- **Schedule Oversight** — List all work weeks (schedules) to understand your staffing coverage and planning.
- **Labor Tracking** — List actual time punches to monitor clock-in/out times and verify labor compliance.
- **Organization Control** — Query business locations, employee roles, and departments to manage your restaurant's structure.
- **Operational Visibility** — Check account status and monitor configured webhooks for real-time schedule events.

### How it works
1. Subscribe to this server
2. Enter your 7shifts Company GUID and Token (found in your developer settings)
3. Start managing your restaurant team from Claude, Cursor, or any MCP client

### Who is it for?
- **Restaurant Managers** — quickly retrieve staff lists and verify shift coverage via simple AI commands.
- **Operations Teams** — create new work assignments and monitor time clock entries directly from the workspace.
- **Business Owners** — get instant bird's-eye views of active shifts and team structure via the AI assistant.


## Available Tools
- **create_employee**: Create a new employee
- **create_shift**: Create a new shift
- **get_account_info**: Get my profile
- **get_employee**: Get employee details
- **list_departments**: List departments
- **list_employees**: List all employees
- **list_locations**: List business locations
- **list_roles**: List employee roles
- **list_schedules**: List all schedules
- **list_shifts**: List all shifts
- **list_time_punches**: List time clock entries
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **7shifts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in my 7shifts account."

**🤖 AI Agent:**
> I've retrieved your employee list. You have 15 active staff members including 'Alex Rivera', 'Sarah Chen', and 'Mike Ross'. Which one would you like to see the shifts for?

---

**👤 You:**
> "Show me the shifts for 'Alex Rivera' (ID: user_10293)."

**🤖 AI Agent:**
> I've fetched the shifts for Alex. He has 3 assignments this week: Tuesday (10:00 - 18:00), Thursday (12:00 - 20:00), and Saturday (08:00 - 16:00). All are scheduled at the 'Downtown' location.

---

**👤 You:**
> "Create a new shift at location 'loc_8823' for tomorrow from 09:00 to 17:00."

**🤖 AI Agent:**
> Success! A new work assignment has been created for tomorrow (09:00 - 17:00) at the Downtown unit. It is currently unassigned. Would you like me to assign an employee to it?


## ❓ FAQ

**Q: Can I see all the active shifts for a specific employee via AI?**
Yes! Use the `list_shifts` tool and provide the optional `user_id`. Your agent will retrieve the complete work history and future assignments for that specific person.

**Q: How do I create a new work shift using the agent?**
Use the `create_shift` action. You'll need to provide the Location ID, and the start and end times in ISO 8601 format (e.g., 2024-12-01T10:00:00Z).

**Q: Is it possible to check real-time clock-in data via AI?**
Absolutely. Use the `list_time_punches` query. The agent will retrieve the history of actual clock-in and clock-out events, allowing you to verify labor compliance instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/7shifts-alternative](https://vinkius.com/mcp/7shifts-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **7shifts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `7shifts-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **7shifts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "7shifts-alternative": {
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
