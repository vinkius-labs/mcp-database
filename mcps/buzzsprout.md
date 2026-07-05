# Buzzsprout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buzzsprout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your podcast via Buzzsprout — track episodes, monitor plays, and manage content directly from any AI agent.

## Description
Connect your **Buzzsprout** account to any AI agent and orchestrate your podcast management, episode creation, and performance tracking through natural conversation.

### What you can do

- **Episode Oversight** — List all your podcast episodes and retrieve detailed metadata, including play counts and audio URLs.
- **Content Management** — Create, update, or delete episodes directly from your workspace with custom titles and descriptions.
- **Performance Tracking** — Monitor all-time play statistics for individual episodes to track your podcast growth.
- **Podcast Information** — Retrieve core podcast details including artwork, website links, and categories.
- **Account Insights** — Access your podcast configuration and settings straight from your workspace.
- **Deep Dives** — Get detailed data for specific episode IDs using natural language.

### How it works

1. Subscribe to this server
2. Enter your Buzzsprout API Token and Podcast ID
3. Start managing your podcast from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Podcasters & Producers** — quickly check episode performance or update show notes without manual dashboard work.
- **Content Marketers** — retrieve episode links and metadata for social media sharing straight from their workflow tools.
- **Developers** — integrate podcast management steps into their environment using natural language.


## Available Tools (7)
- **get_episode**: Get details of a specific episode
- **list_episodes**: List all podcast episodes
- **create_episode**: Create a new podcast episode
- **delete_episode**: Delete an episode permanently
- **get_account_info**: Retrieve core account/podcast settings
- **get_podcast_info**: Retrieve core podcast information
- **update_episode**: Update an existing episode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buzzsprout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 podcast episodes in Buzzsprout."

**🤖 AI Agent:**
> I've retrieved your episodes. Your 5 most recent shows include 'Tech Trends 2026' (ID: ep_1) and 'AI in Daily Life' (ID: ep_2). Both are currently live.

---

**👤 You:**
> "How many plays does the 'Tech Trends 2026' episode have?"

**🤖 AI Agent:**
> Retrieving episode data... 'Tech Trends 2026' has a total of 1,250 plays since it was published on March 15th.

---

**👤 You:**
> "Update the title of episode ep_123 to 'New Improved Title'."

**🤖 AI Agent:**
> Episode ep_123 has been successfully updated with the new title 'New Improved Title' in your Buzzsprout account.


## ❓ FAQ

**Q: Can I check the total play count for an episode using the agent?**
Yes! Use the `get_episode` tool with the Episode ID. Your agent will fetch the detailed metadata, which includes the `total_plays` field for that specific episode.

**Q: How do I update the description of a podcast episode?**
Simply ask the agent to `update_episode` and provide the Episode ID and the new description. The information will be synchronized with Buzzsprout immediately.

**Q: Does the integration allow uploading new audio files?**
Currently, the toolset focuses on managing metadata, status, and analytics. Creating an episode via `create_episode` allows setting the title and description, but the audio file upload should be managed through the Buzzsprout web interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buzzsprout](https://vinkius.com/mcp/buzzsprout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buzzsprout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buzzsprout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buzzsprout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buzzsprout": {
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
