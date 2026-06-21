# Camunda (BPMN Engine) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/camunda-bpmn-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Orchestrate business processes via Camunda — deploy BPMN models, start instances, and manage user tasks directly from any AI agent.

## Description
Connect your **Camunda** engine to any AI agent to automate and monitor complex business workflows through natural language.

### What you can do

- **Process Management** — Deploy BPMN, DMN, or Form resources and start new process instances with custom variables.
- **Human Task Orchestration** — Search for pending user tasks, assign them to specific users, and complete them to move workflows forward.
- **Incident Monitoring** — Identify and inspect process incidents and jobs to troubleshoot bottlenecks or failures in real-time.
- **Definition Inspection** — Retrieve BPMN XML definitions and search through deployed process definitions to understand workflow logic.
- **Cluster Topology** — Monitor the health and topology of your Camunda cluster directly from your conversation.

### How it works

1. Subscribe to this server
2. Enter your Camunda Base URL and Bearer Token
3. Start managing your BPMN workflows from Claude, Cursor, or any MCP-compatible client

No more jumping between the Camunda Modeler and Operate dashboard to check task statuses. Your AI acts as a technical process orchestrator.

### Who is this for?

- **Process Engineers** — instantly check process definitions and deploy updates without leaving the terminal or IDE.
- **Operations Teams** — monitor incidents and manage job failures through simple natural language queries.
- **Developers** — start process instances and complete user tasks during local development and testing flows.


## Available Tools (25)
- **activate_jobs**: Activate (poll) jobs for workers
- **assign_user_task**: Assign a user task to a specific user
- **complete_job**: Complete an activated job
- **complete_user_task**: Complete a user task with variables
- **deploy_resources**: Deploy BPMN, DMN, or Form resources
- **fail_job**: Mark a job as failed (triggers retries or incidents)
- **get_incident**: Get incident details
- **get_process_definition_xml**: Retrieve the BPMN XML of a process definition
- **get_process_instance**: Get details of a specific process instance
- **get_topology**: Get cluster topology and partition status
- **get_user_task_form**: Retrieve the linked form for a user task
- **get_user_task**: Get details of a specific user task
- **get_variable**: Get a specific variable value
- **search_groups**: Search for user groups
- **search_incidents**: Search for process incidents
- **search_jobs**: Search for job instances
- **search_process_definitions**: Search for deployed process definitions
- **search_process_instances**: Search for process instances
- **search_tenants**: Search for tenants (Multi-tenancy)
- **search_user_tasks**: Search for human tasks
- **search_users**: Search for users
- **search_variables**: Search for process or local variables
- **start_process_instance**: Start a new process instance
- **throw_job_error**: Throw a BPMN error from a job
- **unassign_user_task**: Unassign a user task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Camunda (BPMN Engine)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start a new instance of the 'order-fulfillment' process with orderId 550."

**🤖 AI Agent:**
> I've started the process instance for 'order-fulfillment'. The new instance key is 2251799813685249 and it's currently active.

---

**👤 You:**
> "Search for all pending user tasks assigned to 'admin'."

**🤖 AI Agent:**
> I found 3 pending tasks for 'admin'. The most urgent is 'Approve Invoice' (Key: 4503599627370501). Would you like to see the details or complete it?

---

**👤 You:**
> "Show me the BPMN XML for process definition 2251799813685250."

**🤖 AI Agent:**
> Retrieving the BPMN XML... I've fetched the definition. It contains a start event, two service tasks ('Fetch Data', 'Process Payment'), and an end event.


## ❓ FAQ

**Q: Can I start a process instance with specific input data?**
Yes! Use the `start_process_instance` tool and provide the `variables` JSON object. The AI will map your data to the process requirements automatically.

**Q: How do I find all tasks currently assigned to a specific user?**
You can use the `search_user_tasks` tool with a filter like `{"assignee": "user-id"}`. The agent will return a list of all active human tasks for that person.

**Q: Is it possible to see why a process instance is stuck?**
Yes. Use `search_incidents` to find errors in the cluster, and then `get_incident` with the specific key to see the error message and stack trace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/camunda-bpmn-engine](https://vinkius.com/mcp/camunda-bpmn-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Camunda (BPMN Engine)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `camunda-bpmn-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Camunda (BPMN Engine)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "camunda-bpmn-engine": {
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
