# OpenGov MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opengov)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access OpenGov data directly—list reports, query financial funds, and manage users or departments through your AI agent.

## Description
Connect your **OpenGov** account to any AI agent to streamline public sector data management and financial reporting through natural conversation.

### What you can do

- **Reporting & Data** — List available reports, fetch detailed data rows (JSON/CSV), and inspect metadata schemas for precise analysis
- **User Management** — List, create, and update user profiles, roles, and statuses directly from your agent
- **Organizational Structure** — Manage departments and financial funds to track budgetary allocations and institutional hierarchy
- **Resource Inspection** — Fetch specific details for users or funds using unique identifiers

### How it works

1. Subscribe to this server
2. Enter your OpenGov API Key
3. Start querying public sector data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Public Officials** — instantly retrieve budget reports and fund statuses without manual portal navigation
- **Data Analysts** — fetch report schemas and data rows directly into your analysis environment
- **IT Administrators** — manage platform users and departmental structures via simple commands


## Available Tools (11)
- **create_department**: Create a new OpenGov department
- **create_user**: Create a new OpenGov user
- **get_fund**: Get details for a specific OpenGov fund
- **get_report_data**: Get data rows for a specific report
- **get_report_metadata**: Get metadata and schema for a specific report
- **get_user**: Get details for a specific OpenGov user
- **list_departments**: List OpenGov departments
- **list_funds**: List OpenGov funds
- **list_reports**: List available OpenGov reports
- **list_users**: List OpenGov users
- **update_user**: Update an existing OpenGov user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenGov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the reports I have access to in OpenGov."

**🤖 AI Agent:**
> I've retrieved the list of reports. You have access to 'Annual Budget 2024', 'Departmental Expenses', and 'Grant Tracking'. Which one would you like to explore?

---

**👤 You:**
> "Get the data for report ID 'rep-123' in CSV format."

**🤖 AI Agent:**
> Fetching data for report 'rep-123' in CSV format... I've processed the rows. Would you like me to summarize the financial highlights or provide the raw output?

---

**👤 You:**
> "Create a new user with email 'admin@city.gov' as an Admin."

**🤖 AI Agent:**
> I've created the user 'admin@city.gov' with the Admin role. They should now appear in your user list and have access to the platform.


## ❓ FAQ

**Q: How can I retrieve the actual data rows from a specific report?**
Use the `get_report_data` tool with the `report_id`. You can also specify the format (json/csv) and date ranges to filter the results.

**Q: Can I see the structure of a report before pulling the data?**
Yes, use `get_report_metadata` with the `report_id` to see the schema, columns, and structure of the report.

**Q: How do I list all the financial funds available in the platform?**
Run the `list_funds` tool to get a complete list of funds. For more details on a specific fund, use the `get_fund` tool with its ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opengov](https://vinkius.com/mcp/opengov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenGov** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opengov` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenGov** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opengov": {
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
