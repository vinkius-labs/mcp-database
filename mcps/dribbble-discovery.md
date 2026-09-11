# Dribbble Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dribbble-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Dribbble design discovery as an MCP: popular and recent shots, full shot details, designer portfolios, user profiles and design studio teams — official API v2 read-only (OAuth Bearer, 60 req/min).

## Description
**Dribbble** — the showcase community for designers — read-only discovery angle as a single MCP server (the companion dribbble-mcp covers authenticated CRUD for the token owner).

### What you can do
- **Popular shots** — the community's trending design work: UI, illustration, branding, motion
- **Recent shots** — the newest published work for daily inspiration feeds
- **Shot details** — all image sizes, tags, like counts and the designer
- **Designer portfolios** — every published shot of a specific designer
- **Users & teams** — designer profiles and design studio team pages

### Authentication (from the official API v2 docs)
1. Register an app at dribbble.com (account → applications) to get an OAuth2 token with read scope
2. **All v2 calls require the Bearer token** — even public shot listing; anonymous requests return 404 HTML
3. Rate limit: 60 requests/minute (X-Ratelimit headers on every response)

### Who is this for?
Design researchers, moodboard builders, creative agencies, product teams sourcing design references and AI agents that bring design trends into conversations.


## Available Tools (6)
- **get_shot**: Use shot ids from list tools.

Get full details of one shot: images, tags, likes, views, designer
- **list_popular_shots**: Pagination via page/per_page (max 50). Great for moodboards, design research and trend spotting.

List popular shots (trending design work) from the Dribbble community
- **list_recent_shots**: Same payload as popular shots: images, tags, likes, designer. Use for daily inspiration feeds.

List the most recent shots published by the Dribbble community
- **get_user**: Get a Dribbble user profile: bio, location, followers, pro status
- **get_user_shots**: Use user numeric id (from get_user) or username. Great for studying a designer's full style.

List all published shots of a specific Dribbble designer
- **get_team**: Useful to explore studio work and hiring signals.

Get a Dribbble team profile (design studios and agencies)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dribbble Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me this week's most popular dashboard designs"

**🤖 AI Agent:**
> 🎨 **Popular dashboard shots (Dribbble)**

Trending this week:
- SaaS analytics dashboard — dark mode, 2.1k likes
- Fintech portfolio tracker — 1.8k likes
- CRM data table redesign — 1.4k likes

All include hidpi images and tags (dashboard, saas, data-viz). Want me to filter by tag or pull a specific designer's full portfolio?

---

**👤 You:**
> "Show me all shots from the designer behind that iOS app redesign"

**🤖 AI Agent:**
> 🎨 **Designer portfolio (full shot list)**

42 published shots: iOS fintech app (the redesign you saw), travel app concept, icon sets, motion studies...

Consistent visual signature: bold typography, dark gradients. Want the designer's profile stats (followers, pro status)?


## ❓ FAQ

**Q: How do I get the access token?**
Register an application on dribbble.com (your account → applications), then use the OAuth2 authorize flow (https://dribbble.com/oauth/authorize) with your client id/secret to mint a read-scope token. All v2 API calls — even public shot listing — require the Bearer token.

**Q: What is the rate limit?**
60 requests per minute, tracked in the X-Ratelimit-Limit / X-Ratelimit-Remaining / X-Ratelimit-Reset headers of every response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dribbble-discovery](https://vinkius.com/en/ai-agent-connect/dribbble-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dribbble Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dribbble-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dribbble Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dribbble-discovery": {
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
