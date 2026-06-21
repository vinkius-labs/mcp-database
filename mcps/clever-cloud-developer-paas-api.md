# Clever Cloud (Developer PaaS API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clever-cloud-developer-paas-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clever-cloud-developer-paas-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clever-cloud-developer-paas-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Clever Cloud infrastructure—apps, add-ons, and deployments—directly from your AI agent.

## Description
Connect your **Clever Cloud** account to any AI agent and take full control of your PaaS resources through natural conversation.

### What you can do

- **Application Management** — List, create, and inspect your applications. Get detailed metadata and configuration for any specific app.
- **Add-on Provisioning** — List all your provisioned services like databases or Redis, and provision new ones on the fly.
- **Deployment Workflows** — Trigger new deployments for your applications directly from your chat or IDE.
- **Organization Control** — Manage multiple organizations, list their specific applications, and create new organizational units.
- **User Insights** — Retrieve your current user profile and settings to verify access levels.

### How it works

1. Subscribe to this server
2. Enter your Clever Cloud API credentials (Consumer Key, Secret, and Tokens)
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check application statuses and trigger deployments without leaving the terminal or editor.
- **Full-stack Developers** — provision databases (add-ons) and manage app configurations while writing code.
- **Technical Leads** — oversee multiple organizations and applications across the entire Clever Cloud ecosystem.


## Available Tools
- **create_application**: Provide necessary configuration in the body.

Create a new Clever Cloud application
- **create_organization**: Provide configuration in the body.

Create a new organization
- **delete_application**: Delete an application
- **get_addon**: Get details of a specific add-on
- **get_application_logs**: Fetch application logs
- **get_application**: Get details of a specific application
- **get_current_user**: Get information about the current user
- **list_addons**: ).

List all your add-ons
- **list_applications**: List all your Clever Cloud applications
- **list_instances**: List running instances
- **list_organization_applications**: List applications in an organization
- **list_organizations**: List organizations you belong to
- **provision_addon**: Provide configuration in the body.

Provision a new add-on
- **trigger_deployment**: Trigger a deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clever Cloud (Developer PaaS API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Clever Cloud applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'frontend-prod' (ID: app_123), 'api-gateway' (ID: app_456), and 'worker-service' (ID: app_789).

---

**👤 You:**
> "Trigger a new deployment for application app_456."

**🤖 AI Agent:**
> Deployment triggered successfully for 'api-gateway' (app_456). The platform is now building and deploying your latest changes.

---

**👤 You:**
> "Show me the details of my provisioned add-ons."

**🤖 AI Agent:**
> You have 2 active add-ons: a PostgreSQL database (ID: addon_abc) and a Redis instance (ID: addon_xyz). Both are currently in 'running' status.


## Installation & Usage

To install and use the **Clever Cloud (Developer PaaS API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clever-cloud-developer-paas-api](https://vinkius.com/mcp/clever-cloud-developer-paas-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
