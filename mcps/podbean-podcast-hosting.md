# Podbean Podcast Hosting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/podbean-podcast-hosting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your podcasts via Podbean — list episodes, publish new content, and track download analytics directly via AI.

## Description
Connect your AI agent to **Podbean**, the comprehensive podcast hosting and monetization platform. This integration allows you to oversee your podcast catalog, manage episode lifecycles, and audit performance metrics through natural conversation.

### What you can do

- **Episode Management** — List, retrieve, and update details for all your podcast episodes
- **Content Publishing** — Create and publish new episodes or save them as drafts directly via the agent
- **Deep Analytics** — Retrieve download counts and performance trends for entire podcasts or specific episodes
- **Catalog Oversight** — List all podcasts associated with your account and manage their respective IDs
- **Workflow Automation** — Seamlessly delete episodes or update metadata based on listener feedback

### How it works

1. Subscribe to this server
2. Enter your **Podbean Access Token** (obtained from the Podbean Developer Portal)
3. Start managing your podcasting empire through natural language

### Who is this for?

- **Podcasters** — quickly check download stats or publish drafts without opening the dashboard
- **Content Managers** — oversee multiple podcasts and audit episode metadata across different shows
- **Marketing Teams** — track performance trends and identify high-engagement episodes via AI assistance


## Available Tools (8)
- **get_episode_details**: Get comprehensive metadata for a specific podcast episode
- **get_episode_analytics**: Retrieve download analytics for a specific episode
- **get_podcast_analytics**: Retrieve download analytics for a specific podcast
- **list_episodes**: Retrieve a list of episodes for the account
- **list_podcasts**: Retrieve all podcasts associated with the authenticated account
- **publish_episode**: Publish a new podcast episode
- **update_episode**: Update an existing podcast episode
- **delete_episode**: Permanently delete a podcast episode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podbean Podcast Hosting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my podcast episodes."

**🤖 AI Agent:**
> Retrieving episodes... I found several episodes, including 'Episode 1: The Beginning' (Published) and 'Episode 2: Deep Dive' (Draft). Would you like the details for any specific one?

---

**👤 You:**
> "Show me the download analytics for episode ID '12345'."

**🤖 AI Agent:**
> Retrieving analytics for episode '12345'... Total downloads to date: 12,450. Engagement is highest in the first 48 hours after release.


## ❓ FAQ

**Q: How do I get a Podbean Access Token?**
You must register as a developer at the [**Podbean Developer Portal**](https://developers.podbean.com/). Once you create an application, you can use the OAuth 2.0 flow to generate an access token for your account.

**Q: Can I upload audio files through this agent?**
The current version of this MCP server is optimized for metadata management and publishing. For initial audio file uploads, we recommend using the Podbean dashboard to obtain a `media_key`, which can then be used by the agent to publish the episode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podbean-podcast-hosting](https://vinkius.com/mcp/podbean-podcast-hosting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podbean Podcast Hosting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podbean-podcast-hosting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podbean Podcast Hosting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podbean-podcast-hosting": {
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
