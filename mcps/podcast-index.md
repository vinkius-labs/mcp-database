# Podcast Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/podcast-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Access the open podcast ecosystem — search for shows, retrieve episode metadata, and discover trending content directly from your AI agent.

## Description
Connect to the **Podcast Index** to tap into a massive, independent database of podcasts and episodes. This MCP server allows your AI agent to browse the open podcasting directory without the restrictions of proprietary platforms.

### What you can do

- **Deep Search** — Find podcasts by general terms, specific titles, or even by the people (hosts/guests) featured in them.
- **Metadata Retrieval** — Fetch comprehensive details using RSS feed URLs, Index IDs, Podcast GUIDs, or iTunes IDs.
- **Episode Discovery** — List all episodes for a specific feed or find individual episodes by their unique GUID.
- **Trending & Recent** — Stay updated with recent feeds and episodes, or discover something new with random episode selection.

### How it works

1. Subscribe to this server
2. Enter your Podcast Index API Key and Secret
3. Start exploring the world of podcasts from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Researchers** — quickly find episodes on specific topics or featuring certain guests.
- **Developers** — integrate podcast data into applications without building complex scrapers.
- **Podcast Enthusiasts** — discover new shows and stay updated on the latest releases through natural conversation.


## Available Tools (16)
- **get_episode_by_guid**: Get a specific episode by its GUID
- **get_episodes_by_feed_id**: List episodes for a specific feed ID
- **get_episodes_by_feed_url**: List episodes for a specific feed URL
- **get_podcast_by_feed_id**: Get podcast details using its internal Index ID
- **get_podcast_by_feed_url**: Get podcast details using its RSS feed URL
- **get_podcast_by_guid**: Get podcast details using its Podcast GUID
- **get_podcast_by_itunes_id**: Get podcast details using its iTunes ID
- **get_random_episodes**: Get a selection of random episodes
- **get_recent_episodes**: Get the most recently published episodes
- **get_recent_feeds**: Get the most recently added or updated feeds
- **get_recent_new_feeds**: Get feeds newly added to the index
- **get_value_by_feed_id**: Get the value block by feed ID
- **get_value_by_feed_url**: Get the value block (e.g., Lightning Network details) for a feed URL
- **search_by_person**: Search for podcasts featuring a specific person
- **search_by_term**: Search for podcasts by a general search term
- **search_by_title**: Search for podcasts by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podcast Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for podcasts about artificial intelligence using a general term."

**🤖 AI Agent:**
> I've searched the index for 'artificial intelligence'. I found several popular shows including 'The AI Podcast', 'Practical AI', and 'AI in Business'. Would you like the episode list for any of these?

---

**👤 You:**
> "Find all podcasts featuring Lex Fridman."

**🤖 AI Agent:**
> Searching for podcasts associated with Lex Fridman... I found his primary show 'Lex Fridman Podcast' (Feed ID: 750746) and several others where he has appeared as a guest. Should I list the most recent episodes from his main show?

---

**👤 You:**
> "Get the latest episodes for the podcast with feed ID 750746."

**🤖 AI Agent:**
> Fetching episodes for Feed ID 750746... The latest episodes include '#450 – Kevin Hart', '#449 – Donald Trump', and '#448 – Mark Zuckerberg'. Would you like the specific details or GUID for any of these episodes?


## ❓ FAQ

**Q: Can I search for podcasts where a specific person is a guest or host?**
Yes! Use the `search_by_person` tool with the person's name. The agent will return a list of podcasts associated with that individual.

**Q: How do I get the latest episodes from a specific show?**
You can use either `get_episodes_by_feed_id` if you have the internal ID, or `get_episodes_by_feed_url` if you have the RSS link. Both will provide a list of recent episodes.

**Q: Can I find a podcast if I only have its iTunes ID?**
Absolutely. Use the `get_podcast_by_itunes_id` tool to fetch the full Podcast Index metadata using the Apple Podcasts/iTunes identifier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podcast-index](https://vinkius.com/mcp/podcast-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podcast Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podcast-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podcast Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podcast-index": {
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
