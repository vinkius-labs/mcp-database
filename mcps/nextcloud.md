# Nextcloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nextcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Nextcloud instance — handle files, shares, user statuses, and server capabilities directly from your AI agent.

## Description
Connect your **Nextcloud** instance to any AI agent and take full control of your self-hosted productivity suite through natural conversation.

### What you can do

- **File & Folder Management** — List, create, and delete files or folders within your Nextcloud storage directly from the chat.
- **Advanced Sharing** — Create and manage shares for users, groups, or public links with custom permissions and passwords.
- **User & Admin Tools** — List users (admin only), fetch detailed user profiles, and inspect server capabilities and enabled apps.
- **Presence & Status** — Get or set your online status and custom status messages with emojis to keep your team informed.
- **Activity Tracking** — Monitor recent activities and changes within your Nextcloud environment.

### How it works

1. Subscribe to this server
2. Enter your Nextcloud URL, Username, and App Password
3. Start managing your cloud storage and collaboration tools from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Self-Hosters** — Manage your personal cloud infrastructure without leaving your AI workspace.
- **Teams & Organizations** — Quickly share documents and update statuses during collaborative sessions.
- **Developers** — Inspect server capabilities and manage app passwords directly from your coding environment.


## Available Tools (16)
- **get_capabilities**: Get Nextcloud server capabilities
- **create_folder**: Create a new folder in Nextcloud (WebDAV)
- **set_user_status_message**: Set custom user status message
- **set_user_status**: Set user online status
- **create_share**: Share Types: 0=User, 1=Group, 3=Public Link, 4=Email, 6=Federated, 7=Circle, 10=Talk.

Create a new Nextcloud share
- **delete_app_password**: Delete the current app password
- **delete_file**: Delete a file or folder in Nextcloud (WebDAV)
- **delete_share**: Delete a Nextcloud share
- **get_app_password**: Requires authenticating with the real user password.

Generate a new app password
- **get_user_status**: Get current user status
- **get_user**: Get details for a specific Nextcloud user
- **list_activities**: List Nextcloud activity stream
- **list_files**: Path is relative to the user root.

List files in a Nextcloud directory (WebDAV)
- **list_shares**: List all Nextcloud shares
- **list_users**: Requires admin privileges.

List Nextcloud users (Admin only)
- **update_share**: Update an existing Nextcloud share


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nextcloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the capabilities and enabled apps of my Nextcloud server."

**🤖 AI Agent:**
> I've retrieved your server capabilities. You are running Nextcloud 27.1.0. Enabled apps include Files, Photos, Talk, and Calendar. Your server supports large file uploads up to 10GB.

---

**👤 You:**
> "Create a public share link for the folder '/Documents/Project-Alpha' with read-only permissions."

**🤖 AI Agent:**
> I've created the public share for '/Documents/Project-Alpha'. The share ID is 45. You can access it via the generated public link. Permissions are set to Read (1).

---

**👤 You:**
> "Set my status to 'away' and my message to 'Out for lunch' with a pizza emoji."

**🤖 AI Agent:**
> Your status has been updated to 'away' and your custom message is now 'Out for lunch 🍕'.


## ❓ FAQ

**Q: How do I create a public share link for a specific folder?**
Use the `create_share` tool. Provide the `path` to your folder and set `shareType` to 3 (Public Link). You can also optionally set a `password` for added security.

**Q: Can I change my online status message using the AI?**
Yes! You can use `set_user_status` to change your availability (e.g., 'dnd', 'away') and `set_user_status_message` to set a custom text and emoji icon.

**Q: Is it possible to see which apps are enabled on my Nextcloud server?**
Absolutely. Use the `get_capabilities` tool to retrieve a full list of server features, version information, and all currently enabled applications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nextcloud](https://vinkius.com/mcp/nextcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nextcloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nextcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nextcloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nextcloud": {
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
