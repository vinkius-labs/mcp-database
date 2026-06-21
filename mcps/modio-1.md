# Modio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modio-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage game mods and community content via mod.io — list games, browse mods, manage files, and track statistics directly from your AI agent.

## Description
Connect your **mod.io** account to any AI agent and take full control of game mod discovery and management through natural conversation.

### What you can do

- **Game Discovery** — List all games hosted on mod.io and fetch detailed metadata and statistics for specific titles.
- **Mod Management** — Browse mods for any game, add new mods, edit existing ones, or delete content you manage.
- **File & Tag Handling** — List and inspect mod files, manage tags, and explore dependencies to ensure compatibility.
- **User Profile & Subscriptions** — Access your personal profile, list your subscriptions, check your ratings, and manage your mod library.
- **Community Interaction** — Read and add comments, rate mods, and track community engagement metrics.

### How it works

1. Subscribe to this server
2. Enter your mod.io API Key and Access Token
3. Start managing your modding ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — monitor modding activity, manage official content, and track game statistics directly from your workflow.
- **Modders** — upload and update mods, manage files, and respond to community feedback without leaving your IDE.
- **Gaming Communities** — discover new content and manage personal mod collections through simple AI commands.


## Available Tools
- **add_mod_comment**: Add a comment to a mod
- **add_mod_dependencies**: Add dependencies to a mod
- **add_mod_metadata**: Add metadata key-value pairs to a mod
- **add_mod_rating**: Submit a rating for a mod
- **add_mod_tags**: Add tags to a mod
- **add_mod**: Add a new mod to a game
- **checkout_mod**: Purchase a mod
- **delete_mod_comment**: Delete a comment from a mod
- **delete_mod_dependencies**: Delete dependencies from a mod
- **delete_mod_metadata**: Delete metadata key-value pairs from a mod
- **delete_mod_tags**: Delete tags from a mod
- **delete_mod**: Delete a mod
- **edit_mod**: Edit details of an existing mod
- **get_game_stats**: Get statistics for a specific game
- **get_game**: Get details for a specific game
- **list_games**: io.

List all games on mod.io
- **list_my_mods**: Get mods added by the user or where they are a team member
- **list_my_purchased**: Get mods purchased by the authenticated user
- **list_my_ratings**: Get ratings submitted by the authenticated user
- **list_my_subscriptions**: Get mods the authenticated user is subscribed to
- **get_me**: Get authenticated user details
- **list_my_wallets**: Get user wallets and balances
- **list_mod_comments**: List comments for a mod
- **list_mod_dependencies**: List dependencies for a mod
- **get_mod_file**: Get details for a specific mod file
- **list_mod_files**: List all files for a mod
- **list_mod_metadata**: List metadata key-value pairs for a mod
- **get_mod_stats**: Get statistics for a specific mod
- **list_mod_tags**: List tags for a mod
- **list_mod_team**: List team members for a mod
- **get_mod**: Get details for a specific mod
- **list_mods**: List all mods for a specific game
- **subscribe_mod**: Subscribe to a mod
- **list_token_packs**: Get available token packs for a game
- **unsubscribe_mod**: Unsubscribe from a mod


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List games on mod.io with 'Space' in the name."

**🤖 AI Agent:**
> I found several games matching 'Space'. Notable titles include 'Space Engineers' (ID: 164) and 'Space Station 14' (ID: 392). Would you like to see the mods available for any of these?

---

**👤 You:**
> "Show me the most popular mods for game ID 123."

**🤖 AI Agent:**
> Fetching mods for game 123... I've found 10 mods. The top ones are 'HD Textures Pack' and 'Advanced UI Overhaul'. Would you like the details for a specific mod ID?

---

**👤 You:**
> "What are my current mod subscriptions?"

**🤖 AI Agent:**
> Checking your profile... You are currently subscribed to 3 mods: 'Realistic Physics', 'Night Sky Mod', and 'Custom Shaders'. Would you like to check for updates on any of these?


## ❓ FAQ

**Q: How can I check the player statistics for a specific game?**
You can use the `get_game_stats` tool by providing the specific Game ID. The agent will return detailed metrics including total downloads, subscribers, and active mod counts.

**Q: Can I browse my own uploaded mods using this integration?**
Yes! The `list_my_mods` tool allows you to retrieve a list of all mods you have authored or managed on the platform.

**Q: Is it possible to see the files available for a specific mod?**
Absolutely. Use the `list_mod_files` tool with the corresponding Game ID and Mod ID to see all uploaded versions and file details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modio-1](https://vinkius.com/mcp/modio-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Modio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `modio-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Modio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "modio-1": {
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
