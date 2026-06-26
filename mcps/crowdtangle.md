# CrowdTangle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdtangle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to track public social media insights, viral posts, and link shares via the CrowdTangle API.

## Description
Integrate **CrowdTangle**, the public insights tool from Meta, directly into your AI workflow. Monitor social media trends, track how links are being shared across platforms, and identify high-performing content using natural language.

### What you can do

- **Post Monitoring** — List and search for recent public posts on Facebook, Instagram, and other supported platforms.
- **Viral Discovery** — Identify overperforming and viral content based on actual vs. expected interaction.
- **Link Tracking** — See which public accounts and pages have shared specific URLs.
- **Leaderboards & Lists** — Monitor account leaderboards and manage your custom tracking lists.

### How it works

1. Connect the CrowdTangle integration to your AI assistant.
2. Authorize using your CrowdTangle API Token (found in your dashboard Settings).
3. Analyze public social media data and trends through intuitive conversation.

### Who is this for?

- **Journalists & Newsrooms** — Track breaking stories and monitor how news is spreading online.
- **Digital Marketers** — Identify viral trends and audit competitor engagement strategies.
- **Researchers** — Analyze public discourse and link sharing patterns across social platforms.


## Available Tools (10)
- **list_monitored_lists**: Resolves list IDs, names, platform affiliations, and the number of accounts within each list.

List all account lists you are tracking
- **list_media_posts**: Resolves media URLs, content types (Photo, Video), and associated post captions.

List recent posts that contain photos or videos
- **list_recent_posts**: Resolves post content, platform identifiers (Facebook, Instagram, etc.), account names, and engagement metrics (likes, shares, comments).

List recent social media posts tracked by CrowdTangle
- **search_tracking_lists**: Resolves list metadata matching the specified title filter.

Search for specific tracking lists by title
- **search_posts_by_keyword**: Resolves relevant posts, associated accounts, and comparative performance data.

Search for posts across platforms using a keyword
- **get_link_shares**: Resolves which tracked accounts shared the link, their follower counts, and total interactions generated per share.

See which accounts have shared a specific URL
- **get_account_details**: Touches dashboard settings, API rate limits, and workspace configuration boundaries.

Retrieve metadata for your CrowdTangle account
- **get_account_leaderboard**: Resolves account rankings, total interactions, and average engagement rates.

Get engagement leaderboard for accounts in your lists
- **get_post_details**: Touches reaction breakdowns, share history, and platform-specific metadata boundaries.

Get full engagement details for a specific post ID
- **get_top_performing_posts**: Resolves "score" metrics (actual vs expected interactions) and associated social media metadata.

Get the highest performing posts based on actual vs. expected interaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrowdTangle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent viral posts about 'Electric Vehicles' on Instagram."

**🤖 AI Agent:**
> I've found 5 top-performing posts about 'Electric Vehicles'. One post from 'TechDaily' is overperforming by 5x with 12,000 likes and 450 comments. Would you like to see the post URL?

---

**👤 You:**
> "Who has shared the link 'https://vinkius.com/blog/mcp-server' recently?"

**🤖 AI Agent:**
> That link has been shared by 3 public Facebook pages: 'AI News', 'Tech Trends', and 'Developer Hub'. Total interactions from these shares is 1,200. Should I list the individual share details?

---

**👤 You:**
> "Show me the engagement leaderboard for my 'Competitors' list."

**🤖 AI Agent:**
> On your 'Competitors' list, 'Brand X' is currently leading with 45,000 total interactions this week, followed by 'Brand Y' with 32,000. 'Brand Z' saw a 15% dip in engagement. Would you like to see their top post?


## ❓ FAQ

**Q: How do I get a CrowdTangle API Token?**
Log in to your CrowdTangle dashboard, go to **Settings > API**, and you will find your API Token there. Ensure your account has API access enabled.

**Q: Which social platforms are supported?**
CrowdTangle primarily supports Facebook and Instagram public data. It also tracks specific types of data from Reddit and Twitter (limited).

**Q: Can the agent see private accounts?**
No, CrowdTangle only tracks public posts and data from verified pages, groups, and public accounts. Private profiles are not accessible via this API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdtangle](https://vinkius.com/mcp/crowdtangle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrowdTangle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crowdtangle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrowdTangle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crowdtangle": {
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
