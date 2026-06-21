# Doppler MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doppler)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doppler-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doppler-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage secrets and environment variables via Doppler — list projects, audit secrets, and track activity logs from any AI agent.

## Description
Connect your **Doppler** account to any AI agent and take full control of your secrets management through natural conversation.

### What you can do

- **Workspace & Project Discovery** — List all workspaces and projects with their names, slugs and descriptions
- **Config (Environment) Management** — View all configs (development, staging, production) per project and their metadata
- **Secret Auditing** — List all secret names and computed values for any config, with environment fallback resolution
- **Secret Operations** — Add, update and delete secrets in any environment with atomic change requests
- **Activity Logging** — Review the full audit log of secret reads, writes, config changes and user activity per project

### How it works

1. Subscribe to this server
2. Enter your Doppler Service Token or Personal Token
3. Start managing your secrets from Claude, Cursor, or any MCP-compatible client

No more clicking through the Doppler dashboard to check a secret value or audit who changed DATABASE_URL. Your AI acts as a dedicated secrets engineer.

### Who is this for?

- **Developers** — quickly look up secret values for any environment, verify config setups and audit secret inheritance without opening the Doppler UI
- **DevOps Engineers** — review activity logs, audit secret changes and verify project/environment structure for compliance
- **Security Teams** — track who modified which secrets, when and in which environment, enabling full audit trail review via conversation


## Available Tools
- **change_secrets**: Provide project_slug, config_name and a JSON object mapping secret names to values. For example: {"DATABASE_URL":"postgres://...","API_KEY":"sk-..."}. Existing secrets not included are not modified.

Add or update secrets in a Doppler config
- **delete_secrets**: Provide project_slug, config_name and comma-separated secret names. WARNING: deleted secrets cannot be recovered. If a secret inherits a value from a parent, it reverts to that value.

Delete secrets from a Doppler config
- **get_config**: Returns config name, project, root status, associated environment template, creation date and locked status.

Get details for a specific Doppler config
- **get_account**: Returns account email, name, and token metadata (type, scope, permissions). Use this to verify your token is working correctly and understand its access level.

Get the current Doppler account details
- **get_project**: Provide the project slug (e.g. "my-api-project") and optionally the workspace slug.

Get details for a specific Doppler project
- **get_secret**: Returns the secret name and its resolved value with fallbacks from parent environments applied.

Get a specific secret value from a Doppler config
- **list_activity_logs**: Each entry shows who performed what action, when and the affected config. Optionally filter by config_name. Useful for security auditing and compliance.

List activity logs for a Doppler project
- **list_configs**: Each config represents a deployment environment (development, staging, production) and contains its own set of secrets. Returns config name, project slug, root status and environment template used.

List configs (environments) for a Doppler project
- **list_environments**: g. development, staging, production, preview). Returns environment name, slug and whether it is the default environment.

List Doppler environment types
- **list_projects**: Optionally filter by workspace slug. Each project contains configs (environments) and secrets. Returns project name, slug, description, and creation date.

List Doppler projects
- **list_secrets**: Returns each secret's name, computed value (with environment fallbacks applied), visibility status. Provide the project_slug and config_name.

List all secrets for a Doppler config
- **list_workspaces**: A workspace is the top-level organizational unit in Doppler that groups projects. Returns workspace name, slug and creation date.

List all Doppler workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Doppler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all configs for my 'backend-api' project."

**🤖 AI Agent:**
> I found 3 configs for 'backend-api': 'dev' (development, root config), 'staging' (staging, inherits from dev) and 'prod' (production, inherits from staging). Each has its own set of secrets.

---

**👤 You:**
> "Update the DATABASE_URL secret in my prod config to point to the new database."

**🤖 AI Agent:**
> Done! I've updated the `DATABASE_URL` secret in the prod config of your backend-api project. The new value has been applied and will be available to all services using this environment.

---

**👤 You:**
> "Who changed secrets in my project in the last week?"

**🤖 AI Agent:**
> I found 14 activity events in the last 7 days: 3 secret updates by alice@company.com, 8 secret reads by the CI/CD service account, 2 config changes by bob@company.com and 1 new secret added by admin@company.com.


## Installation & Usage

To install and use the **Doppler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doppler](https://vinkius.com/mcp/doppler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
