# itch.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/itchio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access your itch.io account — browse your games, collections and profile info from any AI agent.

## Description
Connect your **itch.io** account to any AI agent and explore your indie game library through natural conversation.

### What you can do

- **Account Info** — View your itch.io profile, username and avatar
- **Your Games** — Browse all games you own, created or collected
- **Collections** — View your game collections and browse games within them
- **Collection Details** — Get games from specific collections by ID

### How it works

1. Subscribe to this server
2. Enter your itch.io API Key
3. Start exploring your game library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers** — browse your itch.io library and discover games in your collections
- **Developers** — check your published games and manage your itch.io presence
- **Curators** — explore collections and organize your game recommendations


## Available Tools (4)
- **get_user_games**: io account including games you've purchased, collected or developed. Returns game titles, URLs, cover images, prices and developer info.

Get games you own or created on itch.io
- **get_collection_games**: io collection by its collection ID. Returns game titles, URLs, cover images, prices and developer info.

Get games in a specific itch.io collection
- **get_me**: io user profile including username, display name, profile URL, avatar URL and cover URL. Use this to verify your API key is working.

Get your itch.io account info
- **get_user_collections**: io. Returns collection names, IDs, game counts and URLs.

Get your itch.io game collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **itch.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my itch.io profile info."

**🤖 AI Agent:**
> Your itch.io profile: Username: gamer123, Display Name: Cool Gamer, Profile URL: https://gamer123.itch.io

---

**👤 You:**
> "What games do I own on itch.io?"

**🤖 AI Agent:**
> You own 15 games on itch.io including: Celeste, Hollow Knight, Undertale, Hades, Stardew Valley, and more. Each with cover images and purchase info.

---

**👤 You:**
> "Show me my itch.io collections."

**🤖 AI Agent:**
> You have 3 collections: "Favorites" (8 games), "Indie Gems" (12 games), "Game Jam Entries" (5 games).


## ❓ FAQ

**Q: How do I get an itch.io API key?**
Log in to [**itch.io**](https://itch.io), go to **User Settings > API Keys** and click **Create API Key**. Give it a name and copy the key immediately.

**Q: What games can I access?**
You can access games you own (purchased or claimed as free), games you've developed, and games in your collections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/itchio](https://vinkius.com/mcp/itchio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **itch.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `itchio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **itch.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "itchio": {
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
