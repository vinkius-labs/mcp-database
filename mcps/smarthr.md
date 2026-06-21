# SmartHR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smarthr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Empower your AI to manage employee records, organizational structures, and payrolls directly from your SmartHR workspace.

## Description
Connect your **SmartHR** directory to any AI agent and empower your team to query employee data, organizational hierarchies, and payroll records securely. Interact with your organization's human capital database through natural language without ever switching tabs.

### What you can do

- **Employee Tracking** — Call the `list_crews` tool to retrieve the roster of all employees and cross-reference demographic metadata
- **Department Hierarchies** — Ask your AI to `list_departments` or check `list_positions` to understand the internal structure
- **Deep Employee Profiles** — Perform targeted queries using `get_crew_details` or `list_crew_dependents` to fetch highly sensitive contract details
- **Payroll Overviews** — Securely query active or historical payroll ledgers to audit compensation scaling

### How it works

1. Subscribe to this server
2. Enter your SmartHR Access Token and Subdomain
3. Start using Claude, Cursor, or any MCP-compatible client to query your employee database

Stop clicking through countless profiles on the SmartHR platform just to find out someone's department or employment type. Your AI agent can read your internal database directly.

### Who is this for?

- **HR Managers & Admins** — easily audit payroll accounts or check an employee's listed dependents internally via chat
- **Department Leads** — request the agent to fetch a list of active job positions and associated team members
- **Security Teams** — check office locations and active employee sublists via the physical `list_establishments` tools


## Available Tools
- **list_crews**: Lists all employees (crews) in SmartHR
- **get_crew_details**: Retrieves details for a specific employee
- **list_departments**: Lists all organizational departments
- **list_positions**: Lists all job positions or roles
- **list_employment_types**: Lists all employment types
- **list_payrolls**: Lists employee payroll records
- **list_establishments**: Lists business establishments or office locations
- **list_crew_dependents**: Lists dependents for a specific employee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SmartHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the entire roster and list the top 3 job positions that occur most frequently."

**🤖 AI Agent:**
> I've fetched the crew and positions. Out of 150 current employees, the top 3 most common job positions in your organization are:
1. Entry-Level Developer (42 members)
2. QA Specialist (18 members)
3. Account Executive (15 members)

---

**👤 You:**
> "Retrieve the details for crew member `crew-8f192`, including their enrolled dependents."

**🤖 AI Agent:**
> Here's the SmartHR profile for Crew `crew-8f192`:
- **Name**: Yuto Tanaka
- **Department**: Engineering Div.
- **Employment Type**: Full-Time Employee

**Dependents Listed**:
- 1 Registered Dependent (Spouse). ID: `dep-43X`

---

**👤 You:**
> "List all physical establishments the company operates."

**🤖 AI Agent:**
> From the endpoint results, your company operates 2 registered business establishments:
1. Tokyo Shibuya Headquarters (Est. Code: HQ-1)
2. Fukuoka Branch Office (Est. Code: FB-2)

Do you want me to map employees to these branches?


## ❓ FAQ

**Q: Is it safe to expose my company's payrolls to the AI?**
Yes. This connector runs entirely on your local machine or trusted enclave natively. No employee data, payload information or generated queries are routed to our servers—your API interactions occur directly from your environment straight to SmartHR's endpoints.

**Q: Can the agent calculate average payroll over time automatically?**
Absolutely. Just prompt your agent: 'List all payrolls from Q2, and display the average distribution'. The agent will call the `list_payrolls` endpoint, retrieve the raw figures, do the mathematical operation independently in context, and present you a very clear table or markdown summary.

**Q: How do I look up which internal department an employee works for?**
You don't need to specify the exact tool. You can simply ask: 'What department is crew member [Name] in?'. Your AI will automatically use the `list_crews` tool and cross reference the results with `list_departments` to formulate a correct response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smarthr](https://vinkius.com/mcp/smarthr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SmartHR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smarthr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SmartHR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smarthr": {
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
