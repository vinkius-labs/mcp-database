# Mastodon Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastodon-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Monitor trending hashtags, viral posts, and community pulse across any Mastodon instance with authenticated API access.

## Description
Access real-time intelligence from any **Mastodon** instance with authenticated API access.

### What you can do

- **Trending Hashtags** — Discover what topics are gaining traction right now with daily and weekly usage counts using `get_trending_hashtags`.
- **Trending Posts** — Surface the most boosted and favourited posts across the network with `get_trending_posts`.
- **Trending Links** — See which external articles and news stories the Fediverse is actively sharing using `get_trending_links`.
- **Public Timeline** — Monitor the live stream of public posts, filtered by local instance or the full federated network.
- **Hashtag Tracking** — Follow specific hashtags like #AI, #OpenSource, or #DevOps to track topic-specific conversations with `get_posts_by_hashtag`.
- **Instance Statistics** — Get community size and activity metrics for your configured instance.

### How it works

1. Subscribe to this server
2. Enter your Mastodon instance URL and access token
3. Start querying trends and timelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — Track organic community sentiment without algorithmic bias.
- **Content Strategists** — Discover trending topics and viral content patterns.
- **Developer Advocates** — Monitor technical conversations across the open web.


## Available Tools (6)
- **get_instance_info**: Use to understand the scale and focus of the Fediverse hub before targeting it for analysis.

Get statistics and description of the configured Mastodon instance
- **get_posts_by_hashtag**: Use to monitor topic-specific conversations on the Fediverse — great for tracking industry hashtags like #AI, #privacy, #journalism, or #OpenSource.

Get the latest public posts for a specific hashtag on Mastodon
- **get_public_timeline**: Use to monitor the real-time conversation pulse of the Fediverse — the open, decentralized social network preferred by journalists, academics, and tech professionals.

Get the latest public posts from Mastodon in real time
- **get_trending_links**: Extremely valuable for content research — it shows what external content the Fediverse community is actively spreading, indicating editorial relevance.

Get the most-shared external links (articles, news) on Mastodon right now
- **get_trending_posts**: Use for content inspiration, sentiment analysis on tech, journalism, and political topics, and understanding what messages spread organically in open social networks.

Get the most boosted and favourited posts on Mastodon right now
- **get_trending_hashtags**: Mastodon trends are algorithm-free and purely usage-based, making them a reliable signal of genuine community interest.

Get trending hashtags on Mastodon right now with weekly history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mastodon Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the top trending hashtags on Mastodon right now?"

**🤖 AI Agent:**
> Here are the top trending hashtags on mastodon.social: #AI (342 uses today), #OpenSource (218 uses), #Privacy (156 uses). These trends are algorithm-free — purely usage-based.

---

**👤 You:**
> "Show me the latest public posts about #DevOps on the Fediverse."

**🤖 AI Agent:**
> Found 15 recent posts with #DevOps. The most engaged post is from @sre_engineer discussing Kubernetes cost optimization with 47 boosts and 89 favourites.

---

**👤 You:**
> "What external articles are being shared the most on Mastodon today?"

**🤖 AI Agent:**
> The top trending links today: 1) 'The EU AI Act explained' from TechCrunch (shared by 89 accounts), 2) 'Open Source funding crisis' from The Register (67 accounts).


## ❓ FAQ

**Q: Do I need a Mastodon account to use this?**
Yes. You need a Mastodon access token with read scope. This guarantees stable rate limits (300 req/5min per account), full compatibility across all instances, and access to trends on instances with restricted public APIs.

**Q: Which Mastodon instance does this monitor?**
By default, mastodon.social — the largest and most active Mastodon instance with over 2 million users. The public timeline also includes federated content from other instances.

**Q: How is this different from the Mastodon MCP?**
The Mastodon MCP requires authentication and lets you post, favourite, follow, and manage your account. This Intelligence MCP is read-only, requires no credentials, and focuses purely on discovery and monitoring — trending topics, public posts, and community insights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastodon-intelligence](https://vinkius.com/mcp/mastodon-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mastodon Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mastodon-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mastodon Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mastodon-intelligence": {
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
