# Harness MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harness)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/harness-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/harness-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Automate CI/CD and DevOps workflows via Harness — manage pipelines, executions, and secrets directly from any AI agent.

## Description
Connect your **Harness.io** platform to any AI agent and take full control of your software delivery and CI/CD pipelines through natural conversation.

### What you can do

- **Pipeline Management** — List, inspect, and trigger pipeline executions across your projects.
- **Execution Monitoring** — Get real-time status updates and step details for active deployments.
- **Project Oversight** — Browse your organizational structure and list projects within specific organizations.
- **Secrets & Infrastructure** — Access lists of secrets, connectors, and environments to ensure your infrastructure is correctly configured.
- **Audit & Compliance** — Retrieve platform audit logs to monitor changes and ensure security standards.
- **Service Insights** — List microservices and environments defined in your DevOps ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Harness API Key, Account ID, and Organization ID
3. Start managing your CI/CD pipelines from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex DevOps dashboards. Your AI assistant acts as a dedicated Release Engineer or DevOps Coordinator.

### Who is this for?

- **DevOps Engineers** — instantly retrieve pipeline statuses and trigger deployments without leaving the IDE.
- **SREs** — monitor execution failures and audit logs to maintain platform stability.
- **Release Managers** — automate the oversight of multiple projects and delivery pipelines.


## Available Tools
- **execute_pipeline**: Trigger the execution of a pipeline
- **get_audit_logs**: Retrieve platform audit logs
- **get_execution_status**: Get status and step details for a specific pipeline execution
- **get_pipeline**: Get details and YAML for a specific pipeline
- **list_connectors**: List infrastructure connectors (Git, Docker, K8s, etc.)
- **list_environments**: List environments defined in a project
- **list_executions**: List executions for a specific pipeline
- **list_pipelines**: List pipelines within a specific project
- **list_projects**: List all projects in the configured Harness organization
- **list_secrets**: List secrets configured in a project
- **list_services**: List services (microservices) defined in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pipelines in project 'E-commerce App'."

**🤖 AI Agent:**
> I've retrieved the pipelines for 'E-commerce App' (ID: app_502). You have 3 active workflows: 'Production Deploy', 'Staging Sync', and 'Security Scan'. Which one would you like to inspect?

---

**👤 You:**
> "Execute the 'Production Deploy' pipeline for project ID app_502."

**🤖 AI Agent:**
> Execution triggered! I've successfully requested the start of 'Production Deploy' (ID: deploy_v1) in project app_502. You can check the status using the `get_execution_status` tool in a few moments.

---

**👤 You:**
> "Show the status of the latest execution for pipeline deploy_v1."

**🤖 AI Agent:**
> Retrieving execution status... The latest execution for 'Production Deploy' (ID: exec_992) is currently IN_PROGRESS. 2 out of 5 steps have completed successfully (Build and Unit Tests). Step 3 (Artifact Push) is running. Should I monitor this for you?


## Installation & Usage

To install and use the **Harness** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harness](https://vinkius.com/mcp/harness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
