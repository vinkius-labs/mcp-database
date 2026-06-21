# Phyllo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phyllo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate creator economy analysis via Phyllo — fetching live creator metrics, cross-platform audience growth, and campaign reach directly from any AI agent.

## Description
Connect your **Phyllo** developer integration to any AI agent and track creator analytics cleanly across dozens of social networks concurrently via natural workflow prompts.

### What you can do

- **Audience Deep Dives** — Query massive, accurate demographics, historical subscriber growth models, and active platform footprints for individual global influencers
- **Campaign Tracking** — Automatically correlate real-time engagement data on live influencer posts scaling directly across YouTube, TikTok, and Instagram
- **Content Aggregation** — Ingest raw video and post performance metadata directly into analytical AI arrays
- **Identity Verification** — Verify social reach legitimately via first-party authenticated account details directly queried from major providers safely

### How it works

1. Subscribe to the Phyllo server deployment here
2. Introduce your Phyllo Client and App secrets provided via their dashboard
3. Engage your LLM dynamically on influencer metrics directly intersecting global arrays

Scale influencer marketing natively without ever scraping manually. Your AI serves as the omniscient engine scoring and reading authentic creator profiles seamlessly.

### Who is this for?

- **Influencer Agencies** — generate pitch documents automatically by querying the most updated engagement footprint available instantly
- **Brand Marketers** — aggregate exact post outputs across sponsored TikTok chains without leaving their enterprise communications
- **Creator Platforms** — verify inbound identity applications for creators bypassing fraud entirely over authenticated loops


## Available Tools (10)
- **create_connect_session**: Generate a secure Connect session token
- **get_account_income**: Fetch verified income streams linked to the creator account
- **get_creator_audience**: Get detailed demographic info about a creators audience
- **get_creator_content**: Retrieve recent posts, videos, or streams from a creator
- **get_creator_profile**: Get a unified creator profile across platforms
- **get_engagement_stats**: Get engagement analytics for a specific piece of content
- **get_identity_status**: Check if a creator has verified their real-world identity
- **get_platform_list**: List all social platforms supported by Phyllo
- **get_webhook_status**: Check the status and configuration of registered webhooks
- **search_creators**: Search for creators across supported social platforms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phyllo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Provide the complete 3-month growth insights for the creator linked to 'uid-9430'."

**🤖 AI Agent:**
> Data fetched successfully. The creator at UID-9430 experienced a 14% overall growth this quarter aggregating platforms. TikTok subscriber acquisition was highest (adding 25k), while YouTube stalled out. Would you like a breakdown of post tags corresponding to the TikTok spike?

---

**👤 You:**
> "List all active posts sponsored by brand XYZ published in the last 48 hours."

**🤖 AI Agent:**
> Scanning campaign outputs... I found 6 affiliated posts across the network mentioning 'Brand XYZ'. 4 are Instagram reels combining for 120k views, and 2 are YouTube integration shorts at 85k views. Are we generating an Excel export of the raw interactions logged so far collectively?

---

**👤 You:**
> "Rank our top 10 verified fitness creators based solely on Instagram comment-to-follower ratio."

**🤖 AI Agent:**
> Applying ratio filter against your creator vault. At the top sits Creator ID 'fit-91', achieving an abnormally high 8% comment ratio despite their large base. Shall I present the entire ranked table mapping out all 10 profiles in markdown seamlessly?


## ❓ FAQ

**Q: Can my AI automatically aggregate all engagement statistics across a specific creator's 3 linked socials?**
Yes! Utilize the `get_creator_identity` combined with `get_audience_metrics`. Your agent will ping Phyllo, mapping their YouTube, TikTok, and Instagram channels simultaneously to produce a single comprehensive metric report instantly.

**Q: How do I easily discover what tier of influencers are trending within the beauty sector?**
Direct your agent to use the `search_creators` tool, filtering via the 'Beauty/Cosmetics' tag and sorting by active engagement. The agent returns ranked creator profiles dynamically bypassing manual research.

**Q: Are there any destructive capabilities regarding a creator's linked accounts?**
No. The API calls are strictly read-only layers fetching authenticated analytical performance or demographic distributions, meaning you cannot post, alter profiles, or delete associations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phyllo](https://vinkius.com/mcp/phyllo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phyllo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phyllo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phyllo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phyllo": {
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
