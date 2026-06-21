# Conductor (Netflix OSS) MCP Server

Automate workflow orchestration via Netflix Conductor — manage workflow and task definitions, and start executions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/conductor-netflix-oss)

## Overview
**Category:** industry-titans
**Tools Count:** 49

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


## Available Tools
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


## Installation & Usage

To install and use the **Conductor (Netflix OSS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conductor-netflix-oss](https://vinkius.com/mcp/conductor-netflix-oss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
