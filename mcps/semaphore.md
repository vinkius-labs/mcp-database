# Semaphore MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semaphore)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/semaphore-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/semaphore-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate CI/CD workflows, manage pipelines, and monitor build jobs directly from your AI agent.

## Description
Connect your **Semaphore CI/CD** account to any AI agent and take full control of your delivery lifecycle through natural conversation.

### What you can do

- **Workflows & Pipelines** — List, run, and stop workflows or pipelines for any project with full visibility into their status.
- **Job Monitoring** — Fetch detailed job information and retrieve logs to debug build failures without leaving your terminal or editor.
- **Deployment & Promotions** — Trigger promotions to different environments and manage deployment targets and history.
- **Artifact Management** — List build artifacts and configure retention policies to keep your storage organized.
- **Agent Management** — Create, update, and monitor agent types and active agents within your organization.

### How it works

1. Subscribe to this server
2. Enter your Semaphore API Token and Organization Slug
3. Start managing your CI/CD pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Monitor pipeline health, rerun failed workflows, and manage deployment targets via chat.
- **Software Developers** — Check build logs and trigger promotions directly from the code editor to maintain flow.
- **Release Managers** — Orchestrate complex deployment sequences and audit deployment history through simple queries.


## Available Tools
- **activate_deployment_target**: Activate a deployment target
- **configure_artifact_retention**: Configure artifact retention policies
- **create_agent_type**: Create a self-hosted agent type
- **create_deployment_target**: Create a deployment target
- **deactivate_deployment_target**: Deactivate a deployment target
- **delete_agent_type**: Delete a self-hosted agent type
- **delete_deployment_target**: Delete a deployment target
- **disable_all_agent_types**: Disable all agents of a specific type
- **get_agent**: Describe a specific self-hosted agent
- **get_agent_type**: Describe a self-hosted agent type
- **get_artifact_retention**: Describe artifact retention policies for a project
- **get_deployment_history**: Get deployment history for a target
- **get_deployment_target_by_name**: Describe a deployment target by name
- **get_deployment_target**: Describe a deployment target by ID
- **get_job_logs**: Get logs for a specific job
- **get_job**: Describe a specific job
- **get_pipeline**: Describe a specific pipeline
- **get_workflow**: Describe a specific workflow
- **list_agent_types**: List self-hosted agent types
- **list_agents**: List self-hosted agents by type
- **list_artifacts**: List artifacts for a scope
- **list_deployment_targets**: List deployment targets for a project
- **list_pipelines**: List pipelines for a project
- **list_promotions**: List promotions for a pipeline
- **list_workflows**: List workflows for a project
- **rebuild_pipeline**: Rebuild failed blocks in a pipeline
- **rerun_workflow**: Rerun a specific workflow
- **run_workflow**: Run a new Semaphore workflow
- **stop_job**: Stop a running job
- **stop_pipeline**: Stop a running pipeline
- **stop_workflow**: Stop a running workflow
- **trigger_promotion**: Trigger a promotion
- **trigger_task**: Trigger a task to run now
- **update_agent_type**: Update a self-hosted agent type
- **update_deployment_target**: Update a deployment target
- **validate_yaml**: Validate a Semaphore pipeline YAML definition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Semaphore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 workflows for project 'api-service'."

**🤖 AI Agent:**
> I've retrieved the latest workflows for project 'api-service'. The most recent one (ID: wf-123) was triggered on 'master' and finished successfully. Would you like to see the pipeline details for any of these?

---

**👤 You:**
> "Show me the logs for job ID 889900 to see why the build failed."

**🤖 AI Agent:**
> Fetching logs for job 889900... The logs indicate a timeout during the 'npm install' step. It seems like a network issue with the registry. Would you like me to rerun the workflow?

---

**👤 You:**
> "Rerun the workflow with ID wf-554433."

**🤖 AI Agent:**
> I have triggered a rerun for workflow wf-554433. A new workflow has been created with ID wf-554434. I'll monitor it for you.


## Installation & Usage

To install and use the **Semaphore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semaphore](https://vinkius.com/mcp/semaphore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
