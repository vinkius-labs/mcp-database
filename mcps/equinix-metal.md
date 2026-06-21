# Equinix Metal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/equinix-metal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/equinix-metal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/equinix-metal-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Equinix Metal API keys, email settings, and project invitations directly from your AI agent.

## Description
Manage your **Equinix Metal** infrastructure access and account settings directly through your AI agent. This server provides tools to handle API keys, email configurations, and project invitations without leaving your conversation.

### What you can do

- **API Key Management** — Create and delete User or Project-level API keys with specific descriptions and read-only permissions.
- **Email Administration** — Add new email addresses to your account, update your default email, or remove old ones.
- **Invitation Handling** — Inspect the details of project invitations and decline them if necessary.

### How it works

1. Subscribe to this server
2. Enter your Equinix Metal API Key
3. Start managing your infrastructure access from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly provision project-specific keys for CI/CD pipelines or temporary access.
- **Infrastructure Leads** — manage team invitations and account communication settings through natural language.
- **Security Teams** — audit and rotate API keys efficiently via AI-driven commands.


## Available Tools
- **create_email**: Create an Email
- **create_project_api_key**: Create a Project API Key
- **create_user_api_key**: Create a User API Key
- **decline_invitation**: Decline an Invitation
- **delete_api_key**: Delete an API Key
- **delete_email**: Delete an Email
- **delete_user_api_key**: Delete a User API Key
- **get_invitation**: View an Invitation
- **update_email**: g., setting it as default).

Update an Email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equinix Metal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new user API key named 'CI-CD-Runner' that is read-only."

**🤖 AI Agent:**
> I've created the user API key 'CI-CD-Runner'. It is set to read-only as requested. The API key ID is 'uuid-123-456'.

---

**👤 You:**
> "Add 'dev-alerts@company.com' to my account emails."

**🤖 AI Agent:**
> I have successfully added 'dev-alerts@company.com' to your account. You may need to verify it in your inbox.

---

**👤 You:**
> "Show me the details for invitation ID 'inv-998877'."

**🤖 AI Agent:**
> Fetching invitation details... This is an invite to join the 'Production-Cluster' project, sent by admin@equinix.com. It expires in 48 hours.


## Installation & Usage

To install and use the **Equinix Metal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/equinix-metal](https://vinkius.com/mcp/equinix-metal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
