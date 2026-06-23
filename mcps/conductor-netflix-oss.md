# Conductor (Netflix OSS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conductor-netflix-oss)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate workflow orchestration via Netflix Conductor — manage workflow and task definitions, and start executions directly from any AI agent.

## Description
Connect your **Netflix Conductor** instance to any AI agent to orchestrate complex microservices and workflows through natural conversation.

### What you can do

- **Workflow Management** — List all registered workflow definitions, fetch specific versions, and manage the lifecycle of your orchestration logic.
- **Task Definitions** — Query and manage the underlying task types that power your microservices, ensuring your workers are correctly configured.
- **Validation & Testing** — Validate workflow JSON definitions before saving them to the server to prevent runtime errors.
- **Execution Control** — Start new workflow instances asynchronously directly from your AI assistant.
- **Batch Operations** — Update or create multiple workflow and task definitions in a single request for rapid deployment.

### How it works

1. Subscribe to this server
2. Enter your Conductor Server URL (e.g., `http://conductor-server:8080`)
3. Start managing your distributed systems from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly inspect and update workflow definitions without navigating the Conductor UI
- **Backend Developers** — validate task configurations and trigger test workflows directly from the IDE
- **System Architects** — visualize and query the structure of complex distributed processes via natural language


## Available Tools (49)
- **add_task_log**: Add a log entry to a task
- **bulk_pause**: Bulk pause workflows
- **bulk_remove**: Bulk remove workflows
- **bulk_restart**: Bulk restart workflows
- **bulk_resume**: Bulk resume workflows
- **bulk_retry**: Bulk retry workflows
- **bulk_search**: Bulk search workflows by ID
- **bulk_terminate**: Bulk terminate workflows
- **create_event_handler**: Create a new event handler
- **create_task_definitions**: Create new task definitions
- **create_workflow_definition**: Create a new workflow definition
- **delete_event_handler**: Delete an event handler
- **delete_task_definition**: Delete a task definition
- **delete_workflow_definition**: Delete a workflow definition
- **execute_workflow**: Execute a workflow (Synchronous)
- **get_all_queues**: Get pending counts for all queues
- **get_correlated_workflows**: Get workflows by correlation ID
- **get_event_handlers**: Get all event handlers
- **get_queue_size**: Get queue depth for a task type
- **get_running_workflows**: Get running workflow IDs by type
- **get_task_definition**: Get a task definition by name
- **get_task_definitions**: Get all task definitions
- **get_task_logs**: Retrieve logs for a task
- **get_workflow_definition**: Get a workflow definition by name
- **get_workflow_definitions**: Get all workflow definitions
- **get_workflow_names_and_versions**: Get all workflow names and versions
- **get_workflow_tasks**: Get tasks for a workflow execution
- **get_workflow**: Get workflow execution by ID
- **pause_workflow**: Pause a workflow
- **poll_batch_tasks**: Long poll for multiple tasks
- **poll_task**: Poll for a single task
- **remove_workflow**: Remove a workflow from the system
- **requeue_tasks**: Requeue pending tasks
- **rerun_workflow**: Rerun a workflow from a specific task
- **restart_workflow**: Restart a workflow from the beginning
- **resume_workflow**: Resume a paused workflow
- **retry_workflow**: Retry the last failed task
- **search_workflows**: Search workflows (returns WorkflowSummary)
- **search_workflows_v2**: Search workflows (returns full Workflow objects)
- **skip_task**: Skip a task in a running workflow
- **start_workflow**: Start a new workflow execution (Asynchronous)
- **terminate_workflow**: Terminate a running workflow
- **update_event_handler**: Update an existing event handler
- **update_task_by_ref**: Update task by reference name
- **update_task_definition**: Update a task definition
- **update_task**: Update task result
- **update_task_v2**: Update task and poll for the next available task
- **update_workflow_definitions**: Create or update workflow definitions (batch)
- **validate_workflow_definition**: Validate a workflow definition without saving


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conductor (Netflix OSS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all workflow names and their versions currently registered in Conductor."

**🤖 AI Agent:**
> I've retrieved the workflow list. You have 3 workflows: 'user_onboarding' (v1, v2), 'payment_processing' (v1), and 'inventory_check' (v1, v2, v3).

---

**👤 You:**
> "Show me the full definition for the workflow 'user_onboarding' version 2."

**🤖 AI Agent:**
> Fetching definition for 'user_onboarding' v2... This workflow consists of 4 tasks: 'verify_email', 'create_profile', 'send_welcome_pack', and 'setup_billing'. Would you like to see the JSON structure?

---

**👤 You:**
> "Start a new execution of the 'payment_processing' workflow."

**🤖 AI Agent:**
> Starting workflow 'payment_processing'... Execution started successfully. The Workflow ID is `8f2b3c4d-5e6f-7a8b-9c0d-1e2f3a4b5c6d`.


## ❓ FAQ

**Q: Can I check if my workflow JSON is valid without saving it to the server?**
Yes! Use the `validate_workflow_definition` tool. It allows you to submit a workflow definition JSON for validation, and the server will return any structural or logic errors without persisting the changes.

**Q: How do I see all available workflows and their versions?**
You can use the `get_workflow_names_and_versions` tool to get a high-level list of all registered workflows and their associated version numbers.

**Q: Is it possible to inspect the configuration of a specific task type?**
Yes, use the `get_task_definition` tool with the specific `taskType` name. This will return the complete task metadata, including retry logic, timeouts, and input/output keys.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conductor-netflix-oss](https://vinkius.com/mcp/conductor-netflix-oss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conductor (Netflix OSS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conductor-netflix-oss` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conductor (Netflix OSS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conductor-netflix-oss": {
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
