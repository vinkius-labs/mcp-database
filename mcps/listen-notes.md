# Listen Notes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/listen-notes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and retrieve podcast and episode metadata via the Listen Notes Podcast API.

## Description
Connect the **Listen Notes Podcast API** to any AI agent to automate your podcast discovery and research workflows. This MCP server enables your agent to search for specific episodes, retrieve complete podcast metadata, explore trending topics, and access curated lists directly from natural language interfaces.

### What you can do

- **Global Podcast Search** — Search for podcasts or individual episodes across the entire database using keywords
- **Episode Insights** — Retrieve complete metadata for any episode, including descriptions, audio links, and transcripts (if available)
- **Discovery & Curation** — Explore best podcasts by genre, access expert-curated lists, and monitor trending search terms
- **Podcast Database Access** — Fetch full show details, publisher information, and chronological episode lists
- **Genre Exploration** — List and query specific categories to identify niche podcast communities

### How it works

1. Subscribe to this server
2. Enter your Listen Notes API Key (X-ListenAPI-Key)
3. Start exploring the world of podcasts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Students** — Quickly find podcast episodes discussing specific academic or industry topics
- **Content Creators** — Monitor trending searches and discover relevant podcasts for competitive research
- **Podcast Enthusiasts** — Automate the discovery of new shows and episodes via simple natural language commands


## Available Tools (7)
- **search_podcasts_or_episodes**: Use the "q" parameter for your query.

Search for podcasts or individual episodes
- **get_trending_podcast_searches**: Get the most recent trending search terms
- **get_best_podcasts**: You can provide an optional genre_id.

Get a list of best podcasts by genre
- **get_curated_podcasts**: Get lists of curated podcasts
- **list_podcast_genres**: List all available podcast genres
- **get_episode_details**: Get metadata for a specific podcast episode
- **get_podcast_details**: Get complete metadata and episodes for a podcast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Listen Notes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for podcast episodes about 'Quantum Computing'."

**🤖 AI Agent:**
> I've searched Listen Notes and found several episodes about Quantum Computing, including 'The Future of Tech' by Science Daily and 'Quantum Explainer' by CodeCast.

---

**👤 You:**
> "What are the trending searches on Listen Notes right now?"

**🤖 AI Agent:**
> The top trending searches include 'Elections 2024', 'AI safety', 'Mental Health', and 'Productivity Hacks'. Would you like to explore results for any of these?

---

**👤 You:**
> "Get details for the podcast with ID '987654321'."

**🤖 AI Agent:**
> I've retrieved the details for the podcast 'Tech Talks'. It is published by 'Innovative Media' and has 150 episodes. The latest episode was published yesterday.


## ❓ FAQ

**Q: Can I filter searches by audio length?**
The current tools support text queries and basic sorting. For advanced filtering like audio length, you can append parameters to the search string or use specific episode details tools.

**Q: How do I find the ID of a specific genre?**
Use the `list_podcast_genres` tool. It returns a full mapping of genre names to their unique numerical IDs.

**Q: Does this server provide audio download links?**
Yes, the `get_episode_details` tool retrieves the metadata including available audio stream URLs and the official website links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listen-notes](https://vinkius.com/mcp/listen-notes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Listen Notes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `listen-notes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Listen Notes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "listen-notes": {
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
