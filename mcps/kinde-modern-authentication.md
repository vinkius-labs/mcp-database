# Kinde (Modern Authentication) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kinde-modern-authentication)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage users, organizations, roles, and permissions in Kinde directly from your AI agent.

## Description
Connect your **Kinde** authentication environment to any AI agent to streamline identity management and access control through natural conversation.

### What you can do

- **User Management** — List all users, create new accounts, retrieve specific profiles, and update user information seamlessly using `list_users`, `create_user`, `get_user`, and `update_user`.
- **Organization Control** — List and create organizations to manage multi-tenant environments with `list_organizations` and `create_organization`.
- **RBAC & Permissions** — Audit available roles and permissions within your Kinde project to ensure proper access control using `list_roles` and `list_permissions`.

### How it works

1. Subscribe to this server
2. Enter your Kinde Domain and Access Token
3. Start managing your auth workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly check user IDs or update test accounts without leaving the IDE
- **Support Teams** — look up user details and organization memberships to troubleshoot access issues
- **DevOps Engineers** — automate the provisioning of organizations and roles through simple prompts


## Available Tools (8)
- **list_roles**: List available roles
- **list_users**: List users in Kinde
- **update_user**: Provide the user ID and the fields to update in the data payload.

Update user information
- **create_organization**: Create a new organization
- **create_user**: Provide user details in the data payload.

Create a new user in Kinde
- **get_user**: Retrieve user details
- **list_organizations**: List organizations in Kinde
- **list_permissions**: List available permissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kinde (Modern Authentication)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Kinde environment."

**🤖 AI Agent:**
> I've retrieved the user list. You have 15 active users. Notable entries include 'John Doe' (ID: kp_123) and 'Jane Smith' (ID: kp_456). Would you like details on a specific user?

---

**👤 You:**
> "Show me all organizations configured in Kinde."

**🤖 AI Agent:**
> Fetching organizations... I found 3 organizations: 'Acme Corp' (org_1), 'Globex' (org_2), and 'Soylent Corp' (org_3).

---

**👤 You:**
> "Get the details for user ID kp_987654321."

**🤖 AI Agent:**
> Inspecting user kp_987654321... This is 'Alice Wonderland'. Email: alice@example.com. Status: Active. Last login: 2 hours ago.


## ❓ FAQ

**Q: Can I create a new user directly through the AI?**
Yes! Use the `create_user` tool by providing the necessary data payload (email, name, etc.). The agent will interface with Kinde to provision the account immediately.

**Q: How do I audit the roles available in my Kinde environment?**
Simply ask the agent to run the `list_roles` tool. It will retrieve all defined roles, allowing you to verify access levels and configurations.

**Q: Is it possible to update an existing user's information?**
Yes, you can use the `update_user` tool. You'll need to provide the `user_id` and the specific fields you wish to modify in the data payload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kinde-modern-authentication](https://vinkius.com/mcp/kinde-modern-authentication)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kinde (Modern Authentication)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kinde-modern-authentication` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kinde (Modern Authentication)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kinde-modern-authentication": {
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
