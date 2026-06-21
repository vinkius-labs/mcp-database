# Deno Deploy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deno-deploy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deno-deploy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deno-deploy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage your Deno Deploy infrastructure — list apps, create deployments, and stream logs directly from your AI agent.

## Description
Connect your **Deno Deploy** account to any AI agent to orchestrate your edge computing infrastructure through natural conversation. This server provides comprehensive tools for managing the lifecycle of your serverless applications.

### What you can do

- **App Management** — List all applications within your organization, filter by labels, and fetch detailed configurations for specific apps.
- **Deployment Lifecycle** — Create new deployments (revisions) by uploading assets, and track their progress in real-time.
- **Log Observability** — Stream build logs for new revisions or query historical application logs with advanced filtering by level and time.
- **Infrastructure Layers** — Manage shared environment variables and configurations using layers to streamline multi-app setups.
- **Domain & Project Insights** — Inspect organization details, list associated domains, and manage project-specific deployments.

### How it works

1. Subscribe to this server
2. Enter your Deno Deploy Personal Access Token
3. Start deploying and monitoring your edge functions from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — automate deployment pipelines and monitor system health without leaving the terminal or chat interface.
- **Full-stack Developers** — quickly check logs or deployment status while debugging code in the IDE.
- **Platform Teams** — manage organizational resources and shared layers across multiple projects efficiently.


## Available Tools
- **create_app**: Create a new Deno Deploy application
- **create_deployment**: Create a new deployment (revision) for an app
- **create_layer**: Create a new layer for sharing environment variables
- **create_project_deployment**: Create a deployment for a project (v1 API)
- **get_app_logs**: Query application logs
- **get_app**: Get details for a specific Deno Deploy app
- **get_build_logs**: Stream build logs for a revision
- **get_organization**: Get organization details (v1 API)
- **get_revision_progress**: Stream revision progress (SSE)
- **get_revision**: Get status of a specific revision
- **list_apps**: Supports pagination and label filtering.

List Deno Deploy applications
- **list_domains**: List custom domains for an organization (v1 API)
- **list_projects**: List projects in an organization (v1 API)
- **list_revisions**: List revisions for an app
- **update_layer**: Update an existing layer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deno Deploy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Deno Deploy apps and show their current status."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'api-gateway' (running), 'web-frontend' (running), and 'auth-service' (deploying). Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the last 50 error logs for the app 'api-gateway'."

**🤖 AI Agent:**
> Fetching logs for 'api-gateway'... I found 12 error entries in the last hour, mostly related to 'Database Connection Timeout'. Would you like me to list the full stack traces?

---

**👤 You:**
> "Check the deployment progress for revision ID 7e8f9a0b."

**🤖 AI Agent:**
> The deployment for revision 7e8f9a0b is currently at the 'Uploading Assets' stage (65% complete). I will continue to monitor the progress for you.


## Installation & Usage

To install and use the **Deno Deploy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deno-deploy](https://vinkius.com/mcp/deno-deploy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
