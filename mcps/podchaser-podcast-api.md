# Podchaser Podcast API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/podchaser-podcast-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Search global podcasts — audit episodes, hosts, and ratings via AI.

## Description
Empower your AI agent to orchestrate your entire audio research and podcast auditing workflow with the **Podchaser Podcast API**, the authoritative source for high-quality audio metadata. By connecting Podchaser to your agent, you transform complex audio searches into a natural conversation. Your agent can instantly search for thousands of podcasts, audit episode lists, and retrieve host metadata without you ever touching a podcast directory. Whether you are conducting media research or managing content distribution constraints, your agent acts as a real-time audio consultant, ensuring your data is always comprehensive and up-to-the-minute.

### What you can do

- **Podcast Auditing** — Search for thousands of podcasts by title or keyword and retrieve detailed metadata, including descriptions and ratings.
- **Episode Oversight** — Audit the complete episode list for any podcast to understand the temporal distribution of audio content instantly.
- **Host Discovery** — Retrieve detailed metadata for podcast hosts and creators to assist in deep-dive media classification.
- **Rating Intelligence** — Query community ratings and reviews to understand the current industry lead in audio quality.
- **Operational Monitoring** — Check API status to ensure your audio research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Podchaser API Key
3. Start managing your audio intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Analysts & Journalists** — monitor podcast trends and retrieve official metadata straight from your workflow.
- **Advertisers & Sponsors** — verify podcast reach and audit audience patterns without manual searching.
- **Content Creators** — perform rapid audits of podcast topics and identify relevant stylistic markers through natural language.
- **Operations Leads** — automate audio data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the Podchaser service is operational
- **get_podcast_details**: Get full metadata and social links for a specific podcast by ID
- **list_podcast_episodes**: List all episodes for a specific podcast ID
- **search_podcasts**: Search for podcasts by title or keywords on Podchaser


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podchaser Podcast API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for podcasts about 'data science' using Podchaser."

**🤖 AI Agent:**
> I've retrieved several podcasts about data science! Notable entries include 'The Data Engineering Podcast' and 'Linear Digressions'. Would you like the full descriptions or the episode list for any of these shows?

---

**👤 You:**
> "What are the latest episodes for podcast ID '12345'?"

**🤖 AI Agent:**
> I've identified the episodes for that podcast! Notable recent titles include [Title 1] and [Title 2], both released in the last week. I can provide the air dates and durations for each of these entries if you'd like.

---

**👤 You:**
> "Show details for podcast 'The Daily'."

**🤖 AI Agent:**
> I've retrieved the details for The Daily! It is currently identified as a 'News' podcast with a high rating. I can provide the unique ID and host metadata to help you identify it in your workflow.


## ❓ FAQ

**Q: How do I find my Podchaser API Key?**
Log in to your [**Podchaser developer portal**](https://api.podchaser.com/), create an application, and you will find your API Token in your dashboard. Copy and paste it below.

**Q: Can I search for podcasts by host?**
Yes. The search tools allow you to use host names as keywords to retrieve podcasts and creators from the Podchaser database.

**Q: Does it support episode descriptions?**
Yes. The `get_podcast_details` and `list_podcast_episodes` tools retrieve detailed descriptions and show notes for podcasts and episodes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podchaser-podcast-api](https://vinkius.com/mcp/podchaser-podcast-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podchaser Podcast API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podchaser-podcast-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podchaser Podcast API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podchaser-podcast-api": {
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
