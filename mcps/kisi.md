# Kisi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kisi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage cloud-based access control, locks, and users via the Kisi API.

## Description
Connect your **Kisi** account to any AI agent to automate your physical access control and security workflows. This MCP server enables your agent to interact with locks (doors), manage users, and trigger remote unlocks directly from natural language interfaces.

### What you can do

- **Remote Unlocking** — Trigger remote unlock commands for any managed door instantly
- **Device Oversight** — List all locks and retrieve real-time status (online/offline, locked/unlocked)
- **User Management** — List organization users and retrieve complete profile information
- **Access Control Audit** — Query groups, places, and role assignments to monitor permissions
- **Location Tracking** — List and inspect physical places configured in your Kisi environment

### How it works

1. Subscribe to this server
2. Enter your Kisi API Key (Personal Access Token)
3. Start managing your facility security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Facilities Managers** — Monitor door statuses and manage access permissions via simple natural language commands
- **Security Teams** — Quickly perform remote unlocks and audit user roles without opening the dashboard
- **Developers** — Integrate physical access control logic and status monitoring into your custom applications


## Available Tools (9)
- **get_lock_details**: Get details for a specific lock
- **get_place_details**: Get details for a specific place
- **list_access_groups**: List all access groups
- **list_locks**: List all locks (doors)
- **get_my_profile**: Get the current authenticated user profile
- **list_places**: List all physical places (locations)
- **list_role_assignments**: List all role assignments
- **unlock_door**: Unlock a specific door (lock)
- **list_users**: Use this to identify user IDs.

List all users in the Kisi organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kisi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Unlock the 'Main Entrance' door (ID: '12345') in Kisi."

**🤖 AI Agent:**
> I've sent the unlock command to 'Main Entrance'. The door should now be unlocked.

---

**👤 You:**
> "List all locks that are currently offline."

**🤖 AI Agent:**
> I've checked your devices. Currently, 'Side Exit (ID: 6789)' and 'Storage Room (ID: 1011)' are reporting as offline.

---

**👤 You:**
> "Show me the details for the place 'Headquarters'."

**🤖 AI Agent:**
> I've retrieved the details for Headquarters (ID: 9876). It currently has 12 active locks and 5 access groups associated with it.


## ❓ FAQ

**Q: How do I perform a remote unlock using the agent?**
Use the `unlock_door` tool with the unique ID of the lock you wish to open. Make sure the authenticated user has the necessary permissions for that door.

**Q: Can I see if a door is currently online?**
Yes, the `list_locks` and `get_lock_details` tools return the real-time connectivity status (online/offline) for every device.

**Q: Is it possible to list all users in my organization?**
Absolutely. Use the `list_users` tool to retrieve a comprehensive list of all members registered in your Kisi organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kisi](https://vinkius.com/mcp/kisi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kisi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kisi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kisi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kisi": {
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
