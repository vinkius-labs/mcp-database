# WorkAdventure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workadventure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create virtual office spaces where remote teams can walk around, bump into colleagues, and collaborate spontaneously.

## Description
Connect your **WorkAdventure** virtual world to any AI agent and simplify how you manage your digital office or event space through natural conversation.

### What you can do

- **Member Management** — List, create, and delete world members to control access to your virtual spaces.
- **World Exploration** — Query maps and active rooms to understand your virtual layout and current occupancy.
- **Room Control** — Get and update room variables to change environmental settings or interactive elements on the fly.
- **World Insights** — Retrieve comprehensive metadata and configuration details about your virtual environment.

### How it works

1. Subscribe to this server
2. Enter your WorkAdventure Admin API Key
3. Start managing your virtual world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Virtual Office Managers** — quickly update office settings, manage team access, and monitor virtual occupancy.
- **Event Organizers** — automate the registration of attendees and change interactive room elements during live sessions.
- **Developers & Designers** — query map metadata and test room variables directly from your workspace via AI.


## Available Tools (10)
- **create_member**: Add a new member to the world
- **delete_member**: Remove a member from the world
- **get_map_details**: Get details of a specific map
- **get_member_details**: Get details of a specific member
- **get_room_variables**: Get variables for a room
- **get_world_info**: Get virtual world information
- **list_maps**: List world maps
- **list_members**: List world members in WorkAdventure
- **list_rooms**: List active rooms
- **update_room_variable**: Update a room variable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WorkAdventure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all registered members in my WorkAdventure world."

**🤖 AI Agent:**
> I've retrieved the member directory. You have 12 registered members, including 'Admin User', 'Guest 01', and 'Developer'. Would you like details on any specific member?

---

**👤 You:**
> "Change the room variable 'welcome_message' to 'Welcome to the Team!' in room 'lobby'."

**🤖 AI Agent:**
> Variable updated successfully! The 'welcome_message' in 'lobby' is now set to 'Welcome to the Team!'. The change should be visible to users in real-time.

---

**👤 You:**
> "Show me a list of all active maps in this world."

**🤖 AI Agent:**
> I found 3 active maps: 'main_office', 'conference_hall', and 'lounge_area'. Each map has its own unique ID and URL for access.


## ❓ FAQ

**Q: Can I change a sign's text in a room using the AI?**
Yes! If the sign is controlled by a room variable, you can use the `update_room_variable` tool to change its value and update the text in real-time.

**Q: How do I see who is currently in my virtual world?**
You can use the `list_members` query to get a directory of all registered members, and `list_rooms` to see active instances and potentially occupancy data.

**Q: Is it possible to grant specific access tags to a new member?**
Absolutely. When using the `create_member` tool, you can provide a comma-separated list of tags to define their permissions and visibility in the world.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workadventure](https://vinkius.com/mcp/workadventure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WorkAdventure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workadventure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WorkAdventure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workadventure": {
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
