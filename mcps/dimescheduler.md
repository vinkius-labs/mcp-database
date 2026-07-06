# Dime.Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dimescheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Plan field service teams visually with drag-and-drop scheduling that connects to your ERP for real-time resource allocation.

## Description
Connect your **Dime.Scheduler** account to any AI agent and take full control of your resource orchestration and project scheduling workflows through natural conversation.

### What you can do

- **Job Orchestration** — List and manage planning jobs programmatically, retrieving detailed metadata about parent entities and project requirements
- **Task Lifecycle Management** — Access and track individual units of work (tasks) that need to be scheduled across your resources in real-time
- **Appointment Monitoring** — List and inspect all appointments on the graphical planning board to maintain a high-fidelity overview of scheduled activities
- **Resource Optimization** — Retrieve complete directories of planable resources (people, equipment, tools) to understand team availability and capacity
- **Category & Marker Intelligence** — Access planning categories and time markers directly through your agent to keep your scheduling board perfectly organized

### How it works

1. Subscribe to this server
2. Retrieve your **X-API-KEY** from your Dime.Scheduler instance settings
3. Start managing your resource planning from Claude, Cursor, or any MCP client

No more manual toggling between complex planning boards or digging through task lists. Your AI acts as your dedicated resource coordinator and scheduling strategist.

### Who is this for?

- **Project Managers** — instantly retrieve job statuses and check task planning across multiple resources using natural language commands
- **Resource Coordinators** — monitor team availability and appointment loads without leaving your communication tools
- **Operations Leads** — track scheduled equipment and maintain board organization through simple AI queries


## Available Tools (7)
- **list_resources**: List all planable resources
- **list_tasks**: List all planning tasks
- **list_time_markers**: List available time markers
- **get_job**: Get job details
- **list_appointments**: List all appointments on the planning board
- **list_categories**: List all planning categories
- **list_jobs**: Scheduler.

List all planning jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dime.Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active planning jobs in Dime.Scheduler."

**🤖 AI Agent:**
> I've retrieved your planning jobs. You currently have 5 active parent entities, including 'Project Alpha' (Job #1024) and 'Maintenance Run'. Which one should we check the tasks for?

---

**👤 You:**
> "Show me all appointments scheduled for tomorrow on the board."

**🤖 AI Agent:**
> Fetching tomorrow's schedule... There are 8 appointments on the planning board, including 4 on-site installations and 2 diagnostic sessions. Would you like the resource details for these?

---

**👤 You:**
> "List all planable resources and their current status."

**🤖 AI Agent:**
> I've retrieved your resource directory. You have 15 available resources, including 10 Technicians (Person), 3 Vans (Tool), and 2 Machines. Shall I check for any overbooked slots today?


## ❓ FAQ

**Q: How do I find my Dime.Scheduler API Key?**
Log in to your Dime.Scheduler instance and navigate to **Settings** > **API** to generate or copy your unique **X-API-KEY**.

**Q: What is the difference between a job and a task?**
A job is the parent project or order, while a task is the specific unit of work that is scheduled on the planning board.

**Q: Can I see real-time team availability?**
Yes! The `list_resources` and `list_appointments` tools allow your agent to identify open slots and currently scheduled work.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dimescheduler](https://vinkius.com/mcp/dimescheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dime.Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dimescheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dime.Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dimescheduler": {
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
