# Railway MCP Server

Equip your AI with direct access to your Railway infrastructure — manage projects, deployments, services, and environment variables.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/railway)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **Railway** cloud infrastructure to an AI agent, streamlining operations directly from your chat terminal. By configuring this integration, the AI gains programmatic management over your active deployments and environments.

### What you can do

- **Project Management** — Create new projects or query existing ones to assess active cloud architectures without opening the web dashboard.
- **Deployment Oversight** — Review build statuses, trigger new deployments, and read rollout logs to ensure stable releases.
- **Service Configuration** — List, update, or restart operational services mapped within your Railway projects securely.
- **Environment Variables** — Manage sensitive configuration keys by securely pulling, updating, or syncing environment values across instances.

### How it works

1. Enable the MCP server integration for Railway.
2. Add your Railway API Token to the configuration.
3. Ask your AI to list projects, fetch deployment health, or handle your services seamlessly.

### Who is this for?

- **DevOps Engineers** — Restart unhealthy containers or verify environment variables quickly from within a VS Code interface.
- **Fullstack Developers** — Trigger deployments after wrapping up a pull request and oversee the operational results interactively.
- **System Administrators** — Conduct fast routine checks on service connectivity scaling without having to rely entirely on separate client applications.


## Available Tools
- **create_project**: Creates a new Railway project
- **delete_project**: This action is irreversible.

Deletes a Railway project
- **get_project**: Retrieves details for a specific Railway project
- **get_service_instances**: Retrieves runtime configuration for a service
- **list_deployments**: Lists deployments for a specific project, environment, and service
- **list_projects**: Lists all Railway projects accessible by the token
- **list_variables**: Lists environment variables for a service
- **restart_service**: Restarts a running service instance
- **trigger_deploy**: Triggers a new deployment for a service
- **whoami**: Retrieves the authenticated Railway user profile


## Installation & Usage

To install and use the **Railway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/railway](https://vinkius.com/mcp/railway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
