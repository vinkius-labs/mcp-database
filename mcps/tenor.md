# Tenor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tenor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Search and discover the world's largest library of GIFs and stickers directly from your AI agent.

## Description
Connect your AI agent to **Tenor** to bring visual expression to your workflows. Access millions of GIFs and stickers, discover trending content, and get smart search suggestions through natural conversation.

### What you can do

- **GIF & Sticker Search** — Find the perfect visual for any emotion or topic using powerful search filters and safety levels.
- **Trending Content** — Stay up to date with global trends by fetching currently featured GIFs and trending search terms.
- **Smart Suggestions** — Get alternative search terms and autocomplete suggestions to refine your visual discovery.
- **Category Exploration** — Browse curated categories like reactions or specific emotions to find exactly what you need.
- **Direct Access** — Retrieve specific GIF metadata and posts using unique IDs for precise sharing.

### How it works

1. Subscribe to this server
2. Enter your Tenor API Key (obtained from Google Cloud Console)
3. Start searching for GIFs in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Find relevant visual content for social media posts and articles without leaving your workspace.
- **Community Managers** — Quickly grab the perfect reaction GIF to engage with your audience.
- **Developers** — Integrate visual search capabilities into your AI-driven applications and chat interfaces.


## Available Tools (8)
- **list_categories**: Retrieve a list of GIF categories
- **get_featured_gifs**: Retrieve the current global featured GIFs
- **get_posts**: Retrieve specific GIFs by their IDs
- **register_share**: Use this when a user explicitly selects/shares a GIF.

Register a share event when a user selects a GIF
- **get_search_suggestions**: Retrieve alternative search terms for a query
- **search_gifs**: Search for GIFs on Tenor
- **get_trending_terms**: Retrieve the current trending search terms
- **get_autocomplete**: Retrieve autocomplete suggestions for a partial search term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tenor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for funny 'victory dance' GIFs on Tenor."

**🤖 AI Agent:**
> I've found several 'victory dance' GIFs for you. Here are the top results, including a celebratory Carlton dance and a joyful animated character. Which one would you like to use?

---

**👤 You:**
> "What are the trending search terms on Tenor right now?"

**🤖 AI Agent:**
> The current trending terms on Tenor include 'Monday motivation', 'happy birthday', 'shocked face', and 'congratulations'. Would you like to see GIFs for any of these?

---

**👤 You:**
> "Give me some search suggestions related to 'coffee'."

**🤖 AI Agent:**
> Based on 'coffee', here are some suggested search terms: 'morning coffee', 'coffee addict', 'iced coffee', and 'need coffee'. Should I search for one of these instead?


## ❓ FAQ

**Q: Can I filter GIF results by safety or content rating?**
Yes! The `search_gifs` and `get_featured_gifs` tools support a `contentfilter` parameter. You can set it to 'off', 'low', 'medium', or 'high' to ensure the results are appropriate for your audience.

**Q: How do I find out what people are currently searching for on Tenor?**
You can use the `get_trending_terms` tool. It returns a list of the most popular search terms currently trending on the platform, helping you stay relevant with current memes and topics.

**Q: Is it possible to retrieve a specific GIF if I already have its ID?**
Absolutely. Use the `get_posts` tool and provide a comma-separated list of GIF IDs. The agent will fetch the full metadata and media formats for those specific items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenor](https://vinkius.com/mcp/tenor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tenor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tenor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tenor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tenor": {
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
