# ShadowBot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shadowbot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate ShadowBot RPA — manage automation robots, handle execution tasks, and monitor bot performance directly from any AI agent.

## Description
Connect your AI agents to **ShadowBot** (影刀RPA), the leading Robotic Process Automation (RPA) platform for high-performance browser and desktop automation. This MCP provides 10 tools to manage automation robots, orchestrate execution tasks, and monitor the health of your digital workforce programmatically.

### What you can do

- **Robot Orchestration** — List and inspect available automation robots and their current operational status
- **Task Execution** — Trigger specific automation tasks and handle job lifecycle management from start to finish
- **Performance Monitoring** — Retrieve granular execution logs and track robot throughput and success rates
- **Credential Handling** — Monitor and manage robotic account assignments and access tokens for secure automation
- **Global Management** — Access organizational project structures and list active automation workflows directly from your agent

### How it works

1. Subscribe to this server
2. Log in to the [**ShadowBot Console**](https://www.winrobot360.com/)
3. Navigate to **API Settings** to obtain your **AppKey** and **AppSecret**
4. Identify your **Organization ID** if applicable for enterprise accounts
5. Insert your credentials into the fields below to start managing your robotic automation workflows.

### Who is this for?

- **RPA Developers** — automate the triggering and monitoring of complex browser/desktop bots
- **Operations Managers** — monitor the performance and health of the digital workforce in real-time
- **Business Analysts** — retrieve execution reports and success metrics via natural language


## Available Tools (10)
- **get_robot_details**: Get detailed information for a specific robot
- **get_task_details**: Retrieve the status and results of a ShadowBot task
- **list_apps**: List all RPA applications in your ShadowBot account
- **list_departments**: Retrieve the organizational department list
- **list_department_members**: List members in a specific department
- **list_online_robots**: List currently online robots
- **list_robots**: List all robots associated with the account
- **list_task_logs**: Retrieve logs for a specific task
- **start_task**: Remote trigger a ShadowBot RPA application
- **stop_task**: Stop a running ShadowBot task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShadowBot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all automation robots in my ShadowBot account and show their status."

**🤖 AI Agent:**
> Retrieving your ShadowBot workforce... I found 3 active robots: 1. WebScraper-01 (Status: Online), 2. DataEntry-02 (Status: Busy), 3. InvoiceProcessor-03 (Status: Offline). Would you like to trigger a task on the online robot?

---

**👤 You:**
> "Start task 'process_invoices' on robot ID 'bot_rpa_777'."

**🤖 AI Agent:**
> Connecting to ShadowBot orchestrator... Success! Job ID `job_999888` has been created for robot 'bot_rpa_777'. The 'process_invoices' workflow is now executing. I will let you know when it completes.

---

**👤 You:**
> "Get the execution logs for Job ID 'job_12345'."

**🤖 AI Agent:**
> Fetching logs for Job `job_12345`... The task completed successfully in 45 seconds. Summary: 15 invoices processed, 0 errors reported. Would you like to see the full JSON output?


## ❓ FAQ

**Q: Can I automatically trigger an RPA task via the AI agent?**
Yes! Use the `trigger_task` tool with the target Robot ID and any required input parameters. Your agent will start the automation job and return the unique Job ID.

**Q: How do I check if a robot is currently online and ready?**
Use the `list_robots` tool. It will retrieve all configured robots in your ShadowBot account along with their current status (e.g., Online, Busy, Offline).

**Q: Can I retrieve the logs for a completed automation job?**
Yes! The `get_task_logs` tool allows you to fetch the execution details and any output data for a specific Job ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shadowbot](https://vinkius.com/mcp/shadowbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShadowBot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shadowbot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShadowBot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shadowbot": {
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
