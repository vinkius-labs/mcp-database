# Are.na Visual Research MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/arena-visual-research)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Are.na as an MCP: search visual research channels, pull blocks (images, links, text, PDFs) with metadata, explore user collections and research thread maps — public v2 API, no key needed for discovery.

## Description
**Are.na** — the visual research and moodboard platform used by designers, artists and researchers — as a single MCP server.

### What you can do
- **Search channels** — curated collections of images, links, text and PDFs on any topic (type design, brutalism, colour theory...)
- **Channel contents** — pull every block: images with metadata, links with descriptions, text excerpts, PDFs
- **User collections** — browse all public channels of any user
- **Research thread maps** — channels connected to a channel: how research topics interlink

### Why Are.na?
Unlike algorithmic feeds, Are.na is human-curated: researchers connect primary sources, articles and images into openly browsable structures. Its public API v2 gives you all of it without keys for public content.

### Who is this for?
Design researchers, artists, curators, trend scouts, moodboard builders and AI agents that need human-curated visual references.


## Available Tools (6)
- **get_channel**: g. "arena-influences"): title, user, follower_count, length (block count), status (public/closed/private). Use slug from search_channels.

Get a channel profile: title, user, collaborator count, block count, status
- **get_channel_contents**: Pagination via per/page. The core research tool for Are.na.

Get the blocks inside a channel: images, links, text, PDFs with metadata
- **list_user_channels**: user id from get_user. slug comes from the channel title slugified (or use the full response).

List all public channels of a user (their research collections)
- **get_user**: user id comes from a channel response (user.id).

Get an Are.na user profile: name, bio, follower counts, channels
- **get_channel_connections**: Shows how research flows across Are.na.

Get connections (blocks linked in from other channels) — the research thread map
- **search_channels**: Channels are curated collections of images, links, text and PDFs. Use slug in get_channel_contents. Pagination via per/page (total_pages returned).

Search public Are.na channels by keyword (visual research collections)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Are.na Visual Research** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Are.na channels about type design"

**🤖 AI Agent:**
> 🧩 **Channel search: type design**

Top results: Type Design (curated collections of typefaces, specimens, foundries)...

Each channel has a slug for pulling its blocks. Want the latest blocks from the biggest channel?

---

**👤 You:**
> "Pull the latest blocks from the Arena Influences channel"

**🤖 AI Agent:**
> 🧩 **Arena Influences (128 blocks, by Charles Broskoski)**

Latest blocks: links to essays, images, PDFs with metadata and content_html for each.

This is the channel that inspired Are.na itself — a research thread map of its connections is available too.


## ❓ FAQ

**Q: Do I need an API key?**
Not for any discovery tool in this MCP — public channel search, contents, users and connections all work without a token. An OAuth2 access token (registered at are.na/apps) is only needed for private channels and write operations.

**Q: What is the API rate limit?**
The public v2 API is rate-limited but generous for research use (per-IP). For heavy integrations, register an OAuth2 app at are.na/apps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/arena-visual-research](https://vinkius.com/en/ai-agent-connect/arena-visual-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Are.na Visual Research** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arena-visual-research` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Are.na Visual Research** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arena-visual-research": {
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
