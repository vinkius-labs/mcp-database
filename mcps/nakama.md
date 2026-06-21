# Nakama MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nakama)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate your game backend via Nakama — manage authentication, user profiles, social features, and storage directly from any AI agent.

## Description
Connect your **Nakama** server to any AI agent to manage your game's backend infrastructure through natural conversation. Nakama is the leading open-source distributed server for social and realtime games and apps.

### What you can do

- **Authentication & Sessions** — Authenticate users via device ID, email, or social providers, and manage active sessions and logouts.
- **User Management** — Fetch and update account profiles, manage wallets, and retrieve public user information.
- **Social & Groups** — Manage friend lists, handle group memberships, and promote or kick members to maintain your community.
- **Storage & Data** — Read, write, and list storage objects to manage player state, inventory, or global game data.
- **Competitive Play** — Access leaderboard records and manage tournament participation directly.
- **Custom Logic** — Execute server-side RPC calls to trigger custom game logic or integrations.

### How it works

1. Subscribe to this server
2. Enter your Nakama Server URL and Session Token
3. Start managing your game backend from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — quickly inspect player data or test backend logic without leaving the IDE.
- **LiveOps Managers** — monitor leaderboards, manage player groups, and handle support requests efficiently.
- **Backend Engineers** — debug storage objects and verify RPC functions through simple natural language queries.


## Available Tools (31)
- **add_friends**: Add friends or send invites
- **add_group_members**: Add members to a group
- **authenticate_device**: Authenticate using a device ID
- **authenticate_email**: Authenticate using email and password
- **block_friends**: Block users
- **create_group**: Create a new group
- **delete_account**: Delete current user account
- **delete_friends**: Remove friends or reject invites
- **delete_storage_objects**: Delete storage objects
- **demote_group_members**: Demote group members
- **get_account**: Fetch current user account
- **get_channel_history**: Get channel message history
- **get_users**: Fetch public user profiles
- **join_group**: Join a group
- **join_tournament**: Join a tournament
- **kick_group_members**: Kick group members
- **leave_group**: Leave a group
- **list_friends**: List friends
- **list_groups**: List groups
- **list_leaderboard_records**: List leaderboard records
- **list_storage_objects**: List storage objects
- **list_tournaments**: List tournaments
- **logout_session**: Logout a session
- **promote_group_members**: Promote group members
- **read_storage_objects**: Read storage objects
- **refresh_session**: Refresh a session token
- **rpc_call**: Call an RPC function
- **update_account**: Update current user account
- **write_leaderboard_record**: Write a leaderboard record
- **write_storage_objects**: Write storage objects
- **write_tournament_record**: Write a tournament record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nakama** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Authenticate a user with email 'player@example.com' and password 'securePass123'."

**🤖 AI Agent:**
> I've initiated the authentication for 'player@example.com'. The session is now active and the user is logged in.

---

**👤 You:**
> "Show me the top records for the 'global_high_scores' leaderboard."

**🤖 AI Agent:**
> Fetching leaderboard data... I've retrieved the top records for 'global_high_scores'. The current leader is 'PlayerOne' with 15,000 points.

---

**👤 You:**
> "List all the groups I am currently a member of."

**🤖 AI Agent:**
> Querying your group memberships... You are currently a member of 3 groups: 'Alpha Squad', 'Beta Testers', and 'The Guild'.


## ❓ FAQ

**Q: Can I register new players using this server?**
Yes. Use `authenticate_email` or `authenticate_device` with the `create` flag set to true. This will register a new account if the credentials don't already exist.

**Q: How do I retrieve a player's virtual wallet or metadata?**
Use the `get_account` tool. It returns the full profile, including the wallet JSON and any linked device identifiers for the authenticated user.

**Q: Can I trigger custom server-side logic?**
Absolutely. Use the `rpc_call` tool by providing the specific Function ID. This allows your AI agent to execute any custom Lua, Go, or TypeScript modules you've deployed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nakama](https://vinkius.com/mcp/nakama)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nakama** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nakama` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nakama** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nakama": {
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
