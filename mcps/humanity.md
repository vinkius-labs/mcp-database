# Humanity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/humanity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workforce scheduling, employee shifts, and team communication via Humanity — list employees, manage locations, and track shifts directly from any AI agent.

## Description
Connect your **Humanity** account to any AI agent to streamline your workforce management and scheduling workflows through natural conversation.

### What you can do

- **Employee Directory** — List all employees, filter by location or position, and retrieve detailed staff profiles
- **Shift Tracking** — Query active shifts and schedules to understand coverage and resource allocation
- **Organizational Structure** — Manage companies, locations, and remote sites to maintain an accurate business hierarchy
- **Position Management** — List and create job positions and roles within your organization
- **User Insights** — Retrieve the authenticated user's profile and permissions to verify access levels

### How it works

1. Subscribe to this server
2. Enter your Humanity Access Token
3. Start managing your workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly audit employee lists and organizational structures without manual exports
- **Operations Leads** — monitor shift coverage and location data directly from your workspace
- **Team Leads** — verify staff assignments and positions to optimize daily operations


## Available Tools (20)
- **list_companies**: List companies
- **get_company**: Get details for a specific company
- **create_location**: Create a new location
- **create_message**: Send a message
- **create_position**: Create a new position
- **create_shift**: Create a new shift
- **create_timeclock_event**: ) to a timeclock.

Add an event to a timeclock
- **create_wall_message**: Post a wall message
- **get_employee**: Get a specific employee
- **list_employees**: List employees
- **list_locations**: List locations or remote sites
- **get_me**: Get current Humanity user details
- **list_positions**: List positions
- **list_shifts**: List shifts
- **terminal_clockin**: Clock in an employee via a terminal
- **list_timeclocks**: List timeclock records
- **get_training_progress**: Get training progress
- **get_training_sections**: Get training sections
- **update_weekly_availability**: Update weekly availability
- **get_weekly_availability**: Get weekly availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Humanity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees assigned to location 55012."

**🤖 AI Agent:**
> I've retrieved the staff list for location 55012. There are 8 employees currently assigned there, including Sarah J. (Manager) and Mike T. (Shift Lead). Would you like the contact details for any of them?

---

**👤 You:**
> "Get the details for company ID 10293."

**🤖 AI Agent:**
> Fetching company details... Company 10293 is 'Global Logistics North'. It currently has 4 active locations and 125 registered employees. Its primary timezone is set to America/New_York.

---

**👤 You:**
> "Create a new position called 'Night Supervisor' at location 8821."

**🤖 AI Agent:**
> The new position 'Night Supervisor' has been successfully created at location 8821. It is currently marked as active. You can now start assigning employees to this role.


## ❓ FAQ

**Q: Can I filter the employee list by a specific location ID?**
Yes! Use the `list_employees` tool and provide the `location` parameter with the target ID. The agent will return only the staff members assigned to that specific site.

**Q: Is it possible to create a new work location through the AI?**
Certainly. You can use the `create_location` action. You'll need to provide a name and type (1 for Location, 2 for Remote Site), and optionally include address and timezone details.

**Q: How do I check the details of my own Humanity account?**
Simply ask the agent to run the `get_me` tool. It will retrieve your current user details, including your profile information and account status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/humanity](https://vinkius.com/mcp/humanity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Humanity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `humanity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Humanity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "humanity": {
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
