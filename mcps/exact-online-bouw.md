# Exact Online Bouw MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exact-online-bouw)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage Dutch construction accounting with project budgets, cost tracking, and financial reporting built for the building industry.

## Description
Connect your **Exact Online Bouw** account to any AI agent and take full control of your construction projects and time tracking workflows through natural conversation.

### What you can do

- **Project Orchestration** — List and manage construction projects programmatically, including creating new entries with account and date metadata
- **Time Tracking Automation** — Register and monitor employee hours for specific projects to maintain a high-fidelity record of labor costs
- **Financial Intelligence** — Programmatically track project costs and expenses to monitor budget utilization and financial health in real-time
- **Structure Visualization** — Access and retrieve Work Breakdown Structures (WBS) to understand project deliverables and activities structured hierarchically
- **Account & Employee Visibility** — Retrieve complete directories of accounts and employees to ensure precise data association for all project entries

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token**, **Division ID**, and **Region** from the Exact Online App Center
3. Start managing your construction projects and hours from Claude, Cursor, or any MCP client

No more manual logging of site hours or complex navigation through ERP tables. Your AI acts as your dedicated construction project and cost coordinator.

### Who is this for?

- **Project Managers** — instantly check project progress and register site hours using natural language commands
- **Finance Teams** — monitor project-specific costs and budget status without leaving your workspace
- **Site Supervisors** — quickly verify employee assignments and project structures through simple AI queries


## Available Tools (12)
- **create_cost_transaction**: Requires project ID, item, date, and amount.

Register a cost or expense for a project
- **create_project**: You can also associate it with an account.

Create a new project in Exact Online
- **create_time_transaction**: Requires project ID, employee ID, item/activity, date, and number of hours.

Register hours (time entry) for a project
- **get_me**: Get current authenticated user and division information
- **get_project**: Get detailed information about a specific project
- **list_accounts**: List accounts (CRM) from Exact Online
- **list_cost_transactions**: List cost transactions registered in Exact Online
- **list_employees**: List employees from Exact Online
- **list_project_hour_budgets**: List hour budgets for projects
- **list_project_wbs**: List the Work Breakdown Structure (WBS) for projects
- **list_projects**: List all projects in Exact Online
- **list_time_transactions**: List time transactions (hours) registered in Exact Online


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exact Online Bouw** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active construction projects in Exact Online."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active works: 'City Tower Renovation' (ID: guid_1), 'Bridge Maintenance' (ID: guid_2), and 'Park Housing'. Which one should I provide the WBS for?

---

**👤 You:**
> "Register 8 hours for employee ID 'emp_123' on 'guid_1' for today."

**🤖 AI Agent:**
> Time entry created! I've registered 8 hours for employee emp_123 on the 'City Tower Renovation' project. The entry is now logged in your Exact Online account for payroll and cost tracking.

---

**👤 You:**
> "How much have we spent on 'City Tower Renovation' so far?"

**🤖 AI Agent:**
> Scanning costs... For the 'City Tower Renovation' (ID: guid_1), total expenses logged so far amount to €15,400.00. This includes materials and labor costs. Would you like a detailed breakdown of these transactions?


## ❓ FAQ

**Q: How do I find my Division ID?**
Use the `get_me` tool to retrieve your current authenticated user profile and the active Division ID associated with your account.

**Q: Can I register hours for a specific date?**
Yes! The `create_time_transaction` tool requires a `Date` parameter in YYYY-MM-DD format to log work entries accurately.

**Q: Which regions are supported for Exact Online?**
Common regions include 'nl', 'be', 'com', 'co.uk'. Check your login URL (e.g., start.exactonline.nl) to confirm your specific region code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exact-online-bouw](https://vinkius.com/mcp/exact-online-bouw)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exact Online Bouw** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exact-online-bouw` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exact Online Bouw** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exact-online-bouw": {
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
