# Grafana Cloud MCP Server

Manage Grafana Cloud organizations, instances, and API keys — list stacks, manage users, and orchestrate observability infrastructure from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana-cloud)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Grafana Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana-cloud](https://vinkius.com/mcp/grafana-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
