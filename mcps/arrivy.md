# Arrivy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arrivy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [field-service-management](../categories/field-service-management.md)

Manage field service tasks, crews, and customer bookings with Arrivy — coordinate last-mile delivery and jobs via AI.

## Description
The **Arrivy MCP Server** empowers your AI agent to coordinate field operations and last-mile delivery directly from your workspace. Seamlessly manage your mobile workforce, track job progress, and engage with customers using natural language.

### Key Features

- **Task Orchestration** — List, create, and update service tasks or delivery jobs with real-time status tracking.
- **Crew Management** — Monitor field personnel and resource assignments to ensure efficient job allocation.
- **Customer Engagement** — Manage customer records and sync service history for better communication.
- **Location Tracking** — Access real-time location data and ETAs for your field technicians and delivery drivers.
- **Digital Workflow** — Access data captured in the field, including forms, photos, and status updates.
- **Seamless Integration** — Connect your Arrivy operations with your AI-assisted project management and support workflows.

### Benefits for Teams

- **Operations Managers** — Quickly audit active jobs and crew statuses without leaving your AI dashboard.
- **Dispatchers** — Use AI to quickly create and assign new tasks based on customer requests.
- **Customer Success** — Retrieve job history and ETAs instantly to provide accurate updates to clients.


## Available Tools (9)
- **create_customer**: Create a new customer record
- **create_task**: Create a new service task in Arrivy
- **get_account_check**: Verify Arrivy account connection
- **get_task**: Get details for a specific task
- **list_crews**: List all field crews and personnel
- **list_customers**: List all customers in the system
- **list_locations**: List all tracked locations
- **list_tasks**: List all service tasks in Arrivy
- **update_task**: Update an existing service task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arrivy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all scheduled tasks for today in Arrivy."

**🤖 AI Agent:**
> I've retrieved your tasks for today. You have 8 scheduled jobs, including 3 'HVAC Repair' tasks and 5 'Package Deliveries'.

---

**👤 You:**
> "Create a new task 'Emergency Leak Repair' at '123 Maple St'."

**🤖 AI Agent:**
> The task 'Emergency Leak Repair' has been successfully created with ID 'task_998877'. Would you like me to assign a crew?

---

**👤 You:**
> "Show me the status of task ID 'T12345'."

**🤖 AI Agent:**
> Task 'T12345' is currently 'In Progress'. The crew arrived at 10:15 AM and is expected to complete the work by 11:30 AM.


## ❓ FAQ

**Q: How do I find my Arrivy API Key?**
Log in to your Arrivy account, go to **Settings > Integrations**, and you will find your API Key under the **Developer** or **API** section.

**Q: Can I assign a crew to a task via this server?**
Yes, you can use the `update_task` tool and provide the crew IDs in the update body to assign or reassign tasks.

**Q: Does Arrivy support real-time ETAs?**
Yes, Arrivy calculates real-time ETAs based on field personnel location. You can retrieve these via the `get_task` or `list_locations` tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arrivy](https://vinkius.com/mcp/arrivy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arrivy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arrivy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arrivy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arrivy": {
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
