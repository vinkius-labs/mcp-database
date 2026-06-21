# Listen Notes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/listen-notes-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and access the world's most comprehensive podcast database — find episodes, podcasts, and curated lists via AI.

## Description
Connect your AI agent to **Listen Notes**, the premier search engine for podcasts. This integration allows you to navigate millions of audio programs and episodes with precision through natural language.

### What you can do

- **Comprehensive Search** — Use the `search` tool to find podcasts, episodes, or curated lists by keywords, genres, or regions.
- **Episode Discovery** — Target specific titles using `search_episode_titles` or fetch deep metadata for a single file via `get_episode`.
- **Podcast Metadata** — Retrieve full show details and episode lists using `get_podcast` or fetch multiple shows at once with `batch_podcasts`.
- **Smart Suggestions** — Use `typeahead` for real-time search suggestions and genre discovery as you type.
- **Transcripts & Details** — Access detailed metadata including descriptions and, for eligible accounts, full episode transcripts.

### How it works

1. Subscribe to this server
2. Enter your Listen Notes API Key
3. Start discovering and analyzing podcast content directly from your MCP-compatible client

### Who is this for?

- **Content Researchers** — quickly find relevant podcast episodes for specific topics or guests
- **Media Analysts** — track podcast appearances and metadata across millions of shows
- **Developers** — integrate podcast discovery and audio metadata into your AI workflows


## Available Tools
- **batch_episodes**: Batch fetch metadata for multiple episodes using their IDs
- **batch_podcasts**: Batch fetch metadata for multiple podcasts
- **create_playlist**: Create or update a playlist
- **get_best_podcasts**: Fetch a list of the best podcasts by genre or region
- **get_episode**: Fetch detailed metadata for a specific episode
- **get_genres**: Fetch a list of all podcast genres and their IDs
- **get_just_listen**: Fetch a random episode (the "I'm Feeling Lucky" of podcasts)
- **get_playlist**: Fetch a curated playlist of episodes or podcasts
- **get_podcast**: Fetch detailed metadata and a list of episodes for a specific podcast
- **get_related_searches**: Fetch search terms related to a specific query
- **get_trending_searches**: Fetch the top 10 most recent trending search terms
- **search_episode_titles**: Targeted search for individual episodes by title
- **search**: Full-text search on episodes, podcasts, or curated lists
- **typeahead**: Suggest search terms, genres, and podcasts as the user types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Listen Notes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for podcasts about 'quantum computing' in English."

**🤖 AI Agent:**
> I found several podcasts about quantum computing. Top results include 'The Quantum Insider' and 'Quantum Computing Now'. Would you like to see the latest episodes for any of these?

---

**👤 You:**
> "Get the details and episode list for podcast ID '4d3fe71774444916851c37235d86a983'."

**🤖 AI Agent:**
> I've retrieved the metadata for 'The Daily'. It currently has 1,500+ episodes. The most recent episode is 'The Sunday Read'. Should I fetch the full description for this episode?

---

**👤 You:**
> "Find an episode titled 'The Future of AI' within the podcast 'Lex Fridman Podcast'."

**🤖 AI Agent:**
> Searching titles... I found the episode 'The Future of AI' in the Lex Fridman Podcast. It was published on May 12th and features Sam Altman. Would you like the full metadata?


## ❓ FAQ

**Q: Can I search for episodes in specific languages or regions?**
Yes. The `search` tool allows you to filter results by `language` and `region` (e.g., 'us', 'gb', 'br') to find content tailored to specific audiences.

**Q: How do I retrieve the full metadata for a specific podcast episode?**
Use the `get_episode` tool with the unique Episode ID. You can also set `show_transcript` to '1' if your Listen Notes plan supports transcripts.

**Q: Is it possible to look up multiple podcasts at once?**
Yes, use the `batch_podcasts` tool. You can provide a comma-separated list of IDs, iTunes IDs, or RSS URLs to fetch metadata for multiple shows in a single request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listen-notes-alternative](https://vinkius.com/mcp/listen-notes-alternative)
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
3. Set Type to "SSE", enter `listen-notes-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Listen Notes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "listen-notes-alternative": {
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
