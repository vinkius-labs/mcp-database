# Infisical MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infisical)
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


## Available Tools (9)
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


## ❓ FAQ

**Q: Is it safe to manage secrets through an AI agent?**
Your credentials are stored encrypted in the Vinkius vault, transmitted only to the Infisical API at runtime. The AI agent never sees raw secret values in its context — only structured operational results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infisical](https://vinkius.com/mcp/infisical)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infisical** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infisical` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infisical** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infisical": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
