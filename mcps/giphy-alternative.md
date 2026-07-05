# Giphy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giphy-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Search, browse, and integrate the world largest library of animated GIFs and stickers into your apps and conversations.

## Description
Connect your **Giphy Developers** account to any AI agent and take full control of your visual media discovery and content curation workflows through natural conversation.

### What you can do

- **Visual Orchestration** — Search across the world's largest library of animated GIFs and transparent stickers programmatically using keywords and precise filters
- **Trending Intelligence** — Monitor real-time trending content globally to keep your social feeds and conversations aligned with current cultural moments
- **Content Translation** — Programmatically translate words or phrases into the single most relevant GIF or sticker using Giphy's internal matching algorithms
- **Metadata Retrieval** — Access granular metadata for specific visual assets, including source URLs, ratings, and dimensions directly through your agent
- **Channel Discovery** — Explore and search through verified Giphy channels to find high-fidelity content from premium brands and creators

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Giphy Developers dashboard (Create an App)
3. Start discovering visual media from Claude, Cursor, or any MCP client

No more manual searching through web interfaces to find the perfect GIF. Your AI acts as your dedicated visual content researcher.

### Who is this for?

- **Social Media Managers** — instantly find trending GIFs for posts and engagement using natural language
- **Product Developers** — integrate dynamic visual content and stickers into applications through automated queries
- **Content Curators** — monitor cultural trends and discover new media assets without leaving your workspace


## Available Tools (10)
- **get_random_sticker**: Get a random sticker
- **search_channels**: Search for Giphy channels
- **search_gifs**: Supports limit, rating, and language.

Search for GIFs
- **search_stickers**: Search for animated stickers
- **translate_text_to_gif**: Translate text to a single GIF
- **translate_text_to_sticker**: Translate text to a sticker
- **get_trending_gifs**: List trending GIFs
- **get_trending_stickers**: List trending stickers
- **get_gif_details**: Get a specific GIF by ID
- **get_random_gif**: Get a random GIF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Giphy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a GIF of 'Space Rocket launch'."

**🤖 AI Agent:**
> Retrieving rocket launch GIFs... I've found 5 high-energy animations. My favorite shows a NASA shuttle liftoff. Would you like the direct link or the source URL?

---

**👤 You:**
> "Show me the top 3 trending GIFs on Giphy right now."

**🤖 AI Agent:**
> Fetching trending content... Currently, the top GIFs include a popular reaction meme, a sports highlight from tonight, and a new movie trailer clip. Which one shall I show you first?

---

**👤 You:**
> "Translate 'Excited for the weekend' into a GIF."

**🤖 AI Agent:**
> Processing translation... Based on Giphy's matching, the perfect GIF for your mood features a happy dance! Here is the asset ID: [id] and the viewing link: [link].


## ❓ FAQ

**Q: How do I get an API Key for Giphy?**
Create a free account at developers.giphy.com and navigate to the dashboard to 'Create an App'. Your key will be displayed in the app settings.

**Q: What is the difference between GIFs and Stickers?**
GIFs are standard animated images. Stickers are animated GIFs with a transparent background, ideal for layering and overlays.

**Q: Can I filter results by content rating?**
Yes! Use the `rating` parameter in the search tools to filter by g, pg, pg-13, or r ratings to ensure appropriate content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giphy-alternative](https://vinkius.com/mcp/giphy-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Giphy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `giphy-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Giphy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "giphy-alternative": {
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
