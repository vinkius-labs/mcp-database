# Buzzsprout MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buzzsprout)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/buzzsprout-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/buzzsprout-mcp)
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


## Available Tools
- **create_episode**: Create a new podcast episode
- **delete_episode**: Delete an episode permanently
- **get_account_info**: Retrieve core account/podcast settings
- **get_episode**: Get details of a specific episode
- **get_podcast_info**: Retrieve core podcast information
- **list_episodes**: List all podcast episodes
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


## Installation & Usage

To install and use the **Buzzsprout** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buzzsprout](https://vinkius.com/mcp/buzzsprout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
