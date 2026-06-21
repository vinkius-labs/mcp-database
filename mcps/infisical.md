# Infisical MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infisical)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/infisical-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/infisical-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage secrets infrastructure via AI — list, create, update, and audit secrets across environments with end-to-end encryption.

## Description
Connect **Infisical** to your AI agent and manage your secrets infrastructure through natural conversation.

### What you can do

- **Secret Management** — List, get, create, update, and delete secrets across any environment
- **Project Overview** — Query project configurations and metadata
- **Environment Navigation** — Browse and switch between dev, staging, and production environments
- **Audit Logging** — Access detailed audit logs for compliance and security tracking
- **Identity Management** — List and manage service identities and access controls

### How it works

1. Subscribe to this server
2. Enter your Infisical Service Token, API URL, Project ID, and environment slug
3. Start managing secrets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — manage secrets across environments without switching context to the dashboard
- **Security Teams** — audit secret access patterns and identity permissions directly from the terminal
- **Platform Engineers** — automate secret rotation and environment configuration workflows


## Available Tools
- **create_secret**: The key must not already exist at that path. Use this to provision new configuration values or credentials.

Create a new secret in the Infisical project
- **delete_secret**: This action cannot be undone. Use with caution.

Delete a secret from the Infisical project
- **get_project_info**: Get information about the configured Infisical project
- **get_secret**: Requires the exact key name as stored in Infisical. Optionally specify a path if the secret is not at the root level.

Get a specific secret by its key name
- **list_audit_logs**: Essential for compliance and security monitoring.

List recent audit log entries for the project
- **list_environments**: g., dev, staging, prod) configured for the project. Use this to discover available environments before switching context.

List all environments in the configured Infisical project
- **list_identities**: Useful for auditing automated access.

List all machine identities configured in the organization
- **list_secrets**: Defaults to the root path "/" if no path is provided. Use this to audit what secrets are available or to verify configuration.

List all secrets in a given path of the current project and environment
- **update_secret**: The key must exist; use create_secret for new entries.

Update the value of an existing secret


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infisical** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all secrets in the production environment."

**🤖 AI Agent:**
> Found 23 secrets in production. Highlights: DATABASE_URL, REDIS_URL, STRIPE_SECRET_KEY, JWT_SECRET. 4 secrets were updated in the last 24 hours. Want to inspect any specific secret?


## Installation & Usage

To install and use the **Infisical** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infisical](https://vinkius.com/mcp/infisical)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
