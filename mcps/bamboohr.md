# BambooHR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bamboohr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Official HR software automation — manage employee directories, time off requests, and company reports via AI.

## Description
Orchestrate your human resources operations with **BambooHR**, the leading platform for small and medium businesses. By connecting BambooHR to your AI agent, you transform complex people management into a natural conversation. Your agent can instantly search the employee directory, audit time off requests, identify who is out of the office today, and retrieve custom company reports without you ever navigating through dense HR menus. Whether you're a manager checking team availability or an HR admin updating records, your agent acts as a direct bridge to your people data, ensuring your organizational culture stays agile and informed.

### What you can do

- **Employee Directory** — Search and list active employees, retrieving basic contact details and profile information through natural language.
- **Time Off Management** — Audit active time off requests, list employees currently out of the office, and submit new requests seamlessly.
- **HR Auditing** — Retrieve specific company reports and list available time off types or policies for your organization.
- **Record Updates** — Programmatically update basic employee information to ensure your HR records are always accurate.
- **Availability Insights** — Quickly identify team members who are out for specific date ranges to optimize project planning.

### How it works

1. Subscribe to this server
2. Enter your BambooHR Subdomain and API Key
3. Start managing your human resources through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Managers** — check who is out of the office today and audit time off requests for your team directly from chat.
- **HR Administrators** — retrieve company reports and update employee records without manual dashboard entry.
- **Operations Leads** — verify employee contact details and organizational structures for project coordination.
- **Knowledge Workers** — quickly find teammates' information and availability through natural conversation.


## Available Tools (12)
- **add_time_off_request**: Submit a new time off request for an employee
- **get_account_check**: Verify BambooHR connection
- **get_company_report**: Get a specific company report by ID
- **get_employee_details**: Get basic details for a specific employee
- **list_employees_directory**: List active employees from the company directory
- **list_time_off_policies**: List all defined time off policies
- **list_time_off_requests**: List time off requests
- **list_time_off_types**: List all defined time off types
- **list_whos_out**: Helper to list who is out today
- **search_employee**: Search for an employee by name in the directory
- **update_employee**: Update employee information
- **whos_out**: List employees who are out (time off) for a date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BambooHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is out of the office today?"

**🤖 AI Agent:**
> Checking BambooHR... Today, Jane Doe (Vacation) and John Smith (Sick Leave) are out. Would you like to check availability for a different date range?

---

**👤 You:**
> "Search for 'Sarah' in the employee directory."

**🤖 AI Agent:**
> I found Sarah Miller. She is a 'Senior Engineer' in the 'Product' team. Her email is sarah.miller@example.com. Would you like her extension or office location?

---

**👤 You:**
> "What are my available time off types?"

**🤖 AI Agent:**
> Retrieving time off types... You have access to: Vacation, Sick Leave, Personal Day, and Bereavement. Which one would you like to request?


## ❓ FAQ

**Q: How do I find a teammate's phone number through the agent?**
Use the `search_employee` tool and provide the teammate's name. Your agent will search the company directory and return their contact details, including phone and email.

**Q: Can the agent tell me who is on vacation today?**
Yes. The `list_whos_out` tool provides a real-time list of all employees who are currently out of the office for time off, allowing you to check team availability instantly.

**Q: Is it possible to submit a time off request via chat?**
Absolutely. Use the `add_time_off_request` tool by providing the employee ID, start and end dates, and the specific Time Off Type ID (e.g., Vacation or Sick Leave).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bamboohr](https://vinkius.com/mcp/bamboohr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BambooHR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bamboohr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BambooHR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bamboohr": {
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
