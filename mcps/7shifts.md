# 7shifts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/7shifts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Restaurant workforce management — manage employee schedules, time-off, and staff profiles via AI.

## Description
Connect your **7shifts** account to your AI agent to streamline restaurant workforce management. From creating weekly schedules to auditing employee time-off requests, your agent handles staffing operations through natural conversation.

### What you can do

- **Employee Management** — List all staff members, create new profiles, and manage employee technical details
- **Scheduling & Shifts** — Create, view, and update work shifts for your entire team across different locations
- **Time-Off Requests** — Audit pending or approved time-off and submit new requests on behalf of employees
- **Labor Tracking** — Access time punch data and monitor clock-in/out patterns for payroll accuracy
- **Location Organization** — Manage multiple restaurant locations, departments, and roles seamlessly

### How it works

1. Subscribe to this server
2. Enter your 7shifts API Key
3. Start managing your restaurant's schedule and staff through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Managers** — build weekly schedules and handle staff changes without manual spreadsheet work
- **Business Owners** — monitor labor costs and employee attendance across multiple locations
- **HR Coordinators** — manage employee records and time-off requests efficiently
- **Operations Leads** — automate staffing reports and schedule notifications


## Available Tools
- **list_employees**: Retrieve all employees registered in the 7shifts company account
- **create_employee**: Requires name and email.

Create a new staff profile inside 7shifts with basic contact information
- **list_shifts**: Retrieve scheduled work shifts from 7shifts, filterable by date or location
- **create_shift**: Requires user_id, location_id, and ISO 8601 start/end times.

Assign a new work shift to a 7shifts employee for a specific date and time
- **list_time_off**: Retrieve pending or approved employee time-off requests from 7shifts
- **list_locations**: Retrieve all locations, departments, and roles configured in the 7shifts account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **7shifts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees for my restaurant."

**🤖 AI Agent:**
> I've retrieved the employee list. You have 25 active staff members including servers, chefs, and hosts. Would you like to see their contact info or roles?

---

**👤 You:**
> "Create a shift for employee 456 on Dec 20th from 9 AM to 5 PM at location 123."

**🤖 AI Agent:**
> Success! I've scheduled the shift for Dec 20th (9:00 - 17:00) at location 123. The employee has been notified through the 7shifts app.

---

**👤 You:**
> "Are there any pending time-off requests?"

**🤖 AI Agent:**
> Checking time-off requests... Yes, you have 3 pending requests: Sarah (Dec 22-24), Mike (Dec 25), and Elena (Jan 2). Would you like to approve any of them?


## ❓ FAQ

**Q: Can I create a new work shift through the agent?**
Yes. Use the `create_shift` tool and provide the employee ID, start/end times, and location ID. Your agent will add the shift to the 7shifts schedule immediately.

**Q: How do I list all restaurant locations?**
Use the `list_locations` tool. Your agent will retrieve all restaurant locations, departments, and roles configured in your 7shifts account.

**Q: Can I see who is currently requesting time off?**
Absolutely. Use the `list_time_off` tool to retrieve all pending and approved time-off requests from your staff for auditing purposes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/7shifts](https://vinkius.com/mcp/7shifts)
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
3. Set Type to "SSE", enter `7shifts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **7shifts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "7shifts": {
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
