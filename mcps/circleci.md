# CircleCI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circleci)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/circleci-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/circleci-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage CI/CD pipelines and workflows via CircleCI — track jobs, trigger pipelines, and monitor build status directly from any AI agent.

## Description
Connect your **CircleCI** account to any AI agent and take full control of your CI/CD pipelines and software delivery through natural conversation. Streamline how you monitor and trigger automated builds.

### What you can do

- **Pipeline Oversight** — List and retrieve details for recent CI/CD pipelines across your organizations natively
- **Trigger Management** — Manually trigger new pipeline runs for specific projects and branches flawlessly
- **Workflow Intelligence** — Access detailed information for workflows and their constituent jobs securely
- **Job Auditing** — Retrieve detailed metadata and execution status for specific jobs flawlessly
- **Context Logistics** — List shared environment contexts used for securing sensitive project data flawlessly
- **Developer Insights** — Retrieve your own user profile and organization membership information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CircleCI Personal API Token (obtained from User Settings)
3. Start managing your pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor pipeline health and trigger manual builds using natural language
- **Software Developers** — audit job failures and review workflow progress without opening the CircleCI dashboard
- **Release Managers** — verify release pipeline status and approve manual gates straight from their chat interface
- **Infrastructure Teams** — manage shared contexts and environment variables across projects


## Available Tools
- **get_my_cci_profile**: Retrieve information about the authenticated user
- **get_workflow_details**: Get detailed information for a specific workflow
- **list_cci_contexts**: List shared contexts for an organization
- **list_workflow_jobs**: List all jobs within a specific workflow
- **list_cci_pipelines**: List recent CI/CD pipelines
- **trigger_cci_pipeline**: Trigger a new pipeline for a project
- **get_job_details**: Get detailed information for a specific job
- **list_pipeline_workflows**: List all workflows within a specific pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CircleCI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 pipelines in CircleCI."

**🤖 AI Agent:**
> Retrieving your recent pipelines... I found 5 items across your projects. 4 were successful and 1 for 'web-app' failed. Would you like to see the workflows for the failed pipeline?

---

**👤 You:**
> "Trigger a new pipeline for project 'gh/acme/api' on the 'main' branch."

**🤖 AI Agent:**
> Triggering pipeline for gh/acme/api (branch: main)... The run has been successfully started. The new pipeline ID is '550e8400-e29b-41d4-a716-446655440000'.

---

**👤 You:**
> "Show me the status of all jobs in workflow ID 'wf-12345'."

**🤖 AI Agent:**
> Checking workflow wf-12345... This workflow has 3 jobs: 'build' (Success), 'test' (Success), and 'deploy' (On Hold). The deploy job is waiting for manual approval.


## Installation & Usage

To install and use the **CircleCI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circleci](https://vinkius.com/mcp/circleci)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
