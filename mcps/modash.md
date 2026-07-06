# Modash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Find and analyze influencers across Instagram, TikTok, and YouTube with Modash.

## Description
Connect **Modash** to your AI agent to discover the perfect creators for your brand. Access a database of 350M+ influencers and get deep audience analytics through natural conversation.

### What you can do

- **Influencer Search** — Find creators based on followers, engagement rate, and location across major platforms.
- **Audience Analytics** — Get detailed reports on audience demographics, location, and authenticity.
- **Platform Coverage** — Seamlessly switch between Instagram, TikTok, and YouTube research.
- **Dictionary Access** — Easily find IDs for locations, interests, and brands to refine your searches.
- **Real-time Data** — Fetch the latest metrics and posts directly from influencer profiles.

### How it works

1. Subscribe to this server
2. Enter your Modash API Token
3. Start discovering influencers with Claude, Cursor, or any MCP client


## Available Tools (11)
- **list_brands**: Search for brand IDs
- **list_interests**: Search for interest IDs
- **list_languages**: Search for language IDs
- **list_locations**: Search for location IDs
- **search_instagram**: Search for Instagram influencers
- **search_tiktok**: Search for TikTok influencers
- **search_youtube**: Search for YouTube channels
- **get_instagram_report**: Get deep analytics for an Instagram profile
- **get_raw_profile**: Get real-time, unfiltered profile data
- **get_tiktok_report**: Get analytics for a TikTok profile
- **get_youtube_report**: Get analytics for a YouTube channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Instagram influencers with 50k-100k followers in London."

**🤖 AI Agent:**
> Searching for influencers... I found 15 matching profiles including @london_lifestyle (72k) and @chef_uk (85k).

---

**👤 You:**
> "Get an audience report for the TikTok user @traveler_vlog."

**🤖 AI Agent:**
> Retrieving report for @traveler_vlog... Audience is 65% female, primarily aged 18-24, located in USA and Brazil.

---

**👤 You:**
> "List all interest categories available for YouTube search."

**🤖 AI Agent:**
> Fetching interests... Popular categories include Gaming, Tech, Beauty, Fashion, and Fitness.


## ❓ FAQ

**Q: Where can I get a Modash API Token?**
You can generate your API token in the Modash Developer Dashboard at https://marketer.modash.io/developer.

**Q: Does Modash support all social media platforms?**
Modash focuses on the big three: Instagram, TikTok, and YouTube.

**Q: Are audience insights real-time?**
Profile reports use high-quality cached data, while the Raw Data tools provide real-time metrics and posts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modash](https://vinkius.com/mcp/modash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Modash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `modash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Modash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "modash": {
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
