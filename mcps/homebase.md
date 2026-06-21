# Homebase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/homebase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate employee scheduling and time tracking via Homebase — manage shifts, locations, and timecards directly from any AI agent.

## Description
Connect your **Homebase** (joinhomebase.com) account to any AI agent and take full control of your employee scheduling, time tracking, and team management through natural conversation.

### What you can do

- **Location Oversight** — List all business locations and retrieve unique identifiers for multi-site management.
- **Employee Management** — Access lists of employees for specific locations and retrieve detailed profile information.
- **Schedule Monitoring** — List scheduled shifts and retrieve upcoming agendas to ensure adequate coverage.
- **Time Tracking** — Monitor actual hours worked by retrieving timecard entries, including clock-in/out times.
- **Real-time Presence** — Instantly check which employees are currently clocked in at a specific location.
- **Role & Department Tracking** — List defined roles and departments to understand your team structure.
- **Operational Efficiency** — Retrieve labor budget configurations to stay aligned with your operational costs.

### How it works

1. Subscribe to this server
2. Enter your Homebase API Key (from Settings > API Access)
3. Start managing your team from Claude, Cursor, or any MCP-compatible client

No more manual exporting of timesheets for simple availability checks. Your AI assistant acts as a dedicated Schedule Coordinator or Operations Manager.

### Who is this for?

- **Store Managers** — instantly check team presence and upcoming shifts without leaving the floor.
- **Operations Leaders** — monitor labor costs and timecard compliance across multiple locations.
- **HR Specialists** — automate the process of retrieving employee profiles and role assignments.


## Available Tools
- **get_active_clock_ins**: List all employees currently clocked in at a specific location
- **get_employee_profile**: Get detailed information for a specific employee
- **get_api_profile**: Retrieve information about the authenticated user and plan status
- **list_departments**: List all departments configured for a location
- **list_employees**: List all employees for a specific location
- **list_labor_budgets**: Retrieve labor budget configurations for a location
- **list_locations**: Use this to find the "location_uuid" required for all other tools.

List all business locations associated with the Homebase account
- **list_defined_roles**: List all roles (e.g., Manager, Server) defined for a location
- **list_scheduled_shifts**: List scheduled shifts for employees at a specific location
- **list_timecards**: Useful for monitoring actual hours worked.

List timecard entries (timesheets) for a specific location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Homebase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all business locations and find the UUID for 'Downtown Cafe'."

**🤖 AI Agent:**
> I've retrieved your locations. You have 3 sites: 'Downtown Cafe' (UUID: hbc_102), 'Airport Kiosk' (UUID: hbc_105), and 'Main Warehouse'. Which location's schedule would you like to check?

---

**👤 You:**
> "Who is currently clocked in at the Downtown Cafe?"

**🤖 AI Agent:**
> Checking active clock-ins for Downtown Cafe (hbc_102)... Currently, 4 employees are on-site: 'Alice Smith' (Barista), 'John Doe' (Manager), 'Michael Brown', and 'Elena Rossi'. Would you like to see their scheduled shift end times?

---

**👤 You:**
> "Show the scheduled shifts for next Wednesday."

**🤖 AI Agent:**
> Retrieving schedules... For next Wednesday (April 14th) at your primary location, 6 shifts are scheduled, starting with 'Morning Prep' at 06:00 AM and ending with 'Closing Duty' at 10:00 PM. Should I list the assigned employees for each shift?


## ❓ FAQ

**Q: How do I obtain my Homebase API Key?**
Log in to Homebase as an Owner, ensure you are on the 'All in One' plan, navigate to **Settings > API Access**, and click **Request API Key**. Your key will typically be approved within one business day.

**Q: Is the Homebase API read-only?**
Yes, as of current documentation, the Homebase public API provides read-only access to locations, employees, timecards, and schedules. Writing data (like creating shifts) must be done through the web dashboard or official POS/Payroll integrations.

**Q: How can I see who is currently working?**
Use the `get_active_clock_ins` tool with your location UUID. It filters current timecards to show only employees who have clocked in but not yet clocked out for the day.

**Q: Is the integration secure for managing employee data?**
Absolutely. The integration uses official Homebase Bearer tokens over HTTPS. Your credentials and sensitive employee information are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/homebase](https://vinkius.com/mcp/homebase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Homebase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `homebase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Homebase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "homebase": {
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
