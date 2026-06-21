# Transistor.fm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transistorfm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/transistorfm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/transistorfm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Host your podcast with analytics, multiple show support, and distribution to Apple Podcasts, Spotify, and every major platform.

## Description
Connect your **Transistor.fm** podcasting account to any AI agent and simplify how you manage your shows, publish new episodes, and grow your audience through natural conversation.

### What you can do

- **Show Management** — List all your podcast shows and retrieve detailed metadata, RSS feeds, and configurations.
- **Episode Workflow** — Create, update, and publish podcast episodes with full control over titles, descriptions, and show notes.
- **Content Curation** — List and search through your entire episode library for any show to manage your publishing history.
- **Private Podcasting** — Manage subscribers for your private shows, including adding new email-based members programmatically.
- **Lifecycle Control** — Delete unwanted episodes or drafts to keep your podcast feed organized.
- **Account Visibility** — Fetch your profile details and verify account settings directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Transistor.fm API Key (found in your account settings)
3. Start managing your podcast empire from Claude, Cursor, or any MCP client

### Who is this for?

- **Podcasters & Producers** — quickly draft show notes and publish episodes via simple AI commands.
- **Content Strategists** — monitor show lists and manage subscriber growth for private podcasts directly from the workspace.
- **Media Teams** — coordinate episode updates and verify publishing statuses via the AI assistant.


## Available Tools
- **add_subscriber**: Add a subscriber to a private podcast
- **create_episode**: Create a new episode
- **delete_episode**: Delete an episode
- **get_episode**: Get details for an episode
- **get_account_details**: fm account.

Get account details
- **get_show**: Get details for a specific show
- **list_episodes**: List episodes for a show
- **list_shows**: List all podcast shows
- **list_subscribers**: List private podcast subscribers
- **publish_episode**: Publish an episode
- **update_episode**: Update an existing episode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transistor.fm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my podcast shows in Transistor.fm."

**🤖 AI Agent:**
> I've retrieved your shows. You have 2 active podcasts: 'The AI Revolution' and 'Tech Builders Weekly'. Which one would you like to manage episodes for?

---

**👤 You:**
> "Show me the last 3 episodes for 'The AI Revolution'."

**🤖 AI Agent:**
> I've fetched the episodes. Here are the 3 most recent: 'S2E01: Future of MCP', 'S1E12: Final Thoughts', and 'S1E11: The GPU Race'. Would you like to update the description for the latest one?

---

**👤 You:**
> "Add 'jane.doe@example.com' as a subscriber to show 'show_10293'."

**🤖 AI Agent:**
> Success! Jane Doe has been added as a subscriber to your private podcast. She will receive her personal invite link shortly.


## Installation & Usage

To install and use the **Transistor.fm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transistorfm](https://vinkius.com/mcp/transistorfm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
