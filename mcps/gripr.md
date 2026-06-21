# Gripr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gripr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Manage safety compliance, inspections, and risk assessments for construction and industrial projects with mobile-first tools.

## Description
Connect your **Gripr (Goliath Systemer)** account to any AI agent and take full control of your construction projects and craft business workflows through natural conversation.

### What you can do

- **Project Orchestration** — List and manage all active construction projects and retrieve detailed technical metadata and status
- **Time Tracking** — Programmatically register work hours for specific projects and retrieve history to ensure accurate billing and labor oversight
- **Task Lifecycle** — Create and manage project tasks to coordinate on-site activities and maintain a high-fidelity project schedule
- **Customer CRM** — Manage customer profiles and retrieve detailed contact information to streamline client communication
- **Field Compliance** — Access HSE (Health, Safety, and Environment) and QA (Quality Assurance) forms directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your API Key from your Gripr account (Settings > Integrations / API)
3. Start managing your construction workflows from Claude, Cursor, or any MCP client

No more manual time logging or complex navigation through fragmented project lists. Your AI acts as your dedicated construction project manager.

### Who is this for?

- **Project Managers** — instantly register site hours and update task statuses using natural language queries
- **Company Owners** — monitor project progress and retrieve customer data without leaving your workspace
- **Field Supervisors** — quickly access compliance forms and manage team assignments across multiple construction sites


## Available Tools (11)
- **create_customer**: Create a new customer
- **create_project**: Create a new project
- **create_task**: Create a new task
- **get_project_details**: Get details for a project
- **list_customers**: List all customers
- **list_forms**: List HSE/QA forms
- **list_registered_hours**: List all registered hours
- **list_projects**: List all projects
- **list_tasks**: Optionally filter by project ID.

List tasks
- **list_workspace_users**: List all users in the workspace
- **register_hours**: Register work hours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gripr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active construction projects."

**🤖 AI Agent:**
> I've retrieved your active projects. You have 3 ongoing works: 'Oslo Waterfront' (ID: p_123), 'Mountain Cabin' (ID: p_456), and 'City Hub' (ID: p_789). Which one would you like to update?

---

**👤 You:**
> "Register 120 minutes of work for project 'p_123' today."

**🤖 AI Agent:**
> Time registered! I've added 120 minutes to the 'Oslo Waterfront' project for today's date. The entry is now logged in your Gripr history for billing.

---

**👤 You:**
> "Show me a list of all customers in Gripr."

**🤖 AI Agent:**
> Scanning customers... I found 5 registered clients, including 'Acme Corp' and 'Global Builders'. Would you like the contact details for any specific customer?


## ❓ FAQ

**Q: How do I find my API Key in Gripr?**
Log in to your Gripr account and navigate to **Settings** > **Integrations / API** to generate your unique key.

**Q: Can I register hours for a specific project?**
Yes! The `register_hours` tool allows you to provide the `projectId`, duration in minutes, and a description for each entry.

**Q: How do I access compliance forms?**
Use the `list_forms` tool to retrieve a directory of all available HSE and QA forms configured in your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gripr](https://vinkius.com/mcp/gripr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gripr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gripr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gripr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gripr": {
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
