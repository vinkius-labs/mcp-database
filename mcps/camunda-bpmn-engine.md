# Camunda (BPMN Engine) MCP Server

Orchestrate business processes via Camunda — deploy BPMN models, start instances, and manage user tasks directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/camunda-bpmn-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 25

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


## Available Tools
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


## Installation & Usage

To install and use the **Camunda (BPMN Engine)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/camunda-bpmn-engine](https://vinkius.com/mcp/camunda-bpmn-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
