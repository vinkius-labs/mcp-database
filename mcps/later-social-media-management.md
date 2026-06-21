# Later (Social Media Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/later-social-media-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage social media via Later — schedule posts, access your media library, and analyze profile performance.

## Description
Connect your **Later** account to any AI agent and take full control of your visual social media planning and multi-profile scheduling through natural conversation.

### What you can do

- **Content Scheduling** — Create and schedule brand new posts across Instagram, TikTok, Pinterest, and LinkedIn with support for custom captions and precise timing directly from your agent
- **Media Library Access** — Browse your central media bank to retrieve uploaded images and videos, including assigned metadata labels and taxonomic classifications
- **Performance Analytics** — Extract aggregated profile metrics (impressions, reach, interactions) over specific date slices to monitor your audience scaling
- **Calendar Orchestration** — Get a global view of your multi-profile content calendar to identify publication gaps and manage your social strategy effectively
- **Queue Management** — List pending scheduled posts and published history to audit your social media presence and selectively delete content before it goes live
- **Workspace Audit** — Retrieve authenticated user info and workspace details to manage collaborative environments and social profile mappings securely

### How it works

1. Subscribe to this server
2. Enter your Later API Token
3. Start managing your social presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — schedule weekly content and monitor performance metrics through natural conversation without jumping between dashboards
- **Content Creators** — manage media assets and track publication histories across multiple social networks directly from your workspace
- **Digital Agencies** — audit global content calendars and manage social profiles for multiple clients efficiently


## Available Tools
- **get_me**: Get authenticated Later user info and workspace details
- **list_profiles**: List connected Later social profiles (Instagram, TikTok, Pinterest, etc)
- **list_media**: Takes standard page index pagination.

List Later media library items
- **list_scheduled_posts**: List pending scheduled posts for a specific Later profile
- **list_published_posts**: List completed published posts including basic performance bounds
- **create_post**: Create and schedule a brand new Later post
- **delete_post**: Delete a Later scheduled post actively pending publication
- **get_analytics**: Get Later aggregated profile analytics spanning an explicit date slice
- **list_labels**: List Later content labels active across the media library
- **get_calendar**: Get the Later global content calendar for a multi-profile date slice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Later (Social Media Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my connected social profiles in Later"

**🤖 AI Agent:**
> I've found 4 connected profiles: 'techcorp_ig' (Instagram, ID: 123), 'techcorp_tt' (TikTok, ID: 456), 'techcorp_pin' (Pinterest, ID: 789), and 'TechCorp_Official' (LinkedIn, ID: 012). Which one would you like to schedule content for?

---

**👤 You:**
> "What posts are scheduled for the coming weekend?"

**🤖 AI Agent:**
> Retrieving calendar for Saturday and Sunday… I've identified 2 posts: 1) Instagram: 'Product Spotlight' (Saturday at 10 AM), 2) TikTok: 'Behind the Scenes' (Sunday at 2 PM). Your calendar looks well-balanced. Would you like to add a Pinterest post?

---

**👤 You:**
> "Show me the performance metrics for my Instagram profile from last month"

**🤖 AI Agent:**
> Retrieving analytics for 'techcorp_ig'… Last month, you achieved 125,400 total impressions, reached 45,200 unique accounts, and had 3,850 total interactions (likes, comments, saves). This is a 12% increase compared to the previous month. Great progress!


## ❓ FAQ

**Q: Can I schedule posts for different social networks at once?**
Yes. The `create_post` tool allows you to specify a profile ID. You can command your agent to create multiple posts targeting different profiles (e.g., Instagram and TikTok) sequentially using the same or different captions.

**Q: How do I see my upcoming scheduled content across all profiles?**
Use the `get_calendar` tool and provide a date range (start and end dates). Your agent will retrieve the global content calendar, identifying all structural post boundaries across your entire Later account.

**Q: Can my agent retrieve analytics for a specific time period?**
Absolutely. The `get_analytics` tool allows your agent to fetch rolled-up metrics like impressions and reach for a specific profile between two dates, providing a rapid summary of your social performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/later-social-media-management](https://vinkius.com/mcp/later-social-media-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Later (Social Media Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `later-social-media-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Later (Social Media Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "later-social-media-management": {
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
