# Equinix Metal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/equinix-metal)
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


## Available Tools (9)
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


## ❓ FAQ

**Q: Can I create a read-only API key for a specific project?**
Yes! Use the `create_project_api_key` tool. You can specify the `project_id`, a description, and set the `read_only` flag to true to ensure the key has restricted permissions.

**Q: How do I manage the email addresses associated with my account?**
You can use `create_email` to add a new address, `update_email` to change settings like the default status, and `delete_email` to remove an address from your profile.

**Q: Is it possible to view and decline project invitations via AI?**
Yes. Use `get_invitation` to see the details of a pending invite and `decline_invitation` if you do not wish to join that specific project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/equinix-metal](https://vinkius.com/mcp/equinix-metal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equinix Metal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equinix-metal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equinix Metal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equinix-metal": {
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
