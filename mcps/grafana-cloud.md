# Grafana Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/grafana-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/grafana-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage Grafana Cloud organizations, instances, and API keys — list stacks, manage users, and orchestrate observability infrastructure from your AI agent.

## Description
Connect your **Grafana Cloud** account to any AI agent to streamline your observability workflows and infrastructure management through natural language.

### What you can do

- **Organization Management** — List all organizations you belong to and fetch deep metadata for specific org slugs.
- **Stack & Instance Control** — Retrieve all Grafana instances (stacks) within an organization and create new ones (Free or Pro plans) on the fly.
- **User Administration** — Audit and list all users belonging to your cloud organizations to maintain access control.
- **API Key Lifecycle** — List, create, and delete API keys with specific roles (Viewer, Editor, Admin) directly from your conversation.
- **Infrastructure Inspection** — Get precise details for specific instances to understand your deployment status without leaving your terminal or editor.

### How it works

1. Subscribe to this server
2. Enter your Grafana Cloud API Key (Cloud Access Policy token)
3. Start managing your observability stacks from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & SREs** — quickly audit stacks, check user lists, and provision new instances without navigating the Cloud Portal UI.
- **Platform Engineers** — automate the creation of API keys and instances as part of developer onboarding or CI/CD flows.
- **Security Teams** — monitor and rotate API keys across multiple organizations using simple AI commands.


## Available Tools
- **create_api_key**: Create a new API key
- **create_instance**: Create a new instance (stack)
- **delete_api_key**: Delete an API key
- **get_instance**: Get details for a specific instance
- **get_org**: Get details for a specific organization
- **list_api_keys**: List API keys for an organization
- **list_instances**: List all instances (stacks) in an organization
- **list_org_users**: List users in an organization
- **list_orgs**: List organizations you belong to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grafana Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Grafana Cloud organizations."

**🤖 AI Agent:**
> I've retrieved your organizations. You have access to: 'Main-Ops' (slug: main-ops) and 'Dev-Sandbox' (slug: dev-sandbox). Which one would you like to explore?

---

**👤 You:**
> "Show me all instances in the 'main-ops' organization."

**🤖 AI Agent:**
> In the 'main-ops' organization, I found 2 instances: 'Production-Stack' (URL: main-ops.grafana.net) and 'Staging-Metrics' (URL: main-ops-staging.grafana.net).

---

**👤 You:**
> "Create an Admin API key named 'automation-token' for the 'dev-sandbox' org."

**🤖 AI Agent:**
> Successfully created the API key 'automation-token' with Admin role. The key is: `glc_...`. Please store it securely as it won't be shown again.


## Installation & Usage

To install and use the **Grafana Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana-cloud](https://vinkius.com/mcp/grafana-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
