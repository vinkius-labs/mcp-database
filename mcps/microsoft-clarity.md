# Microsoft Clarity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-clarity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

See exactly how users interact with your website through heatmaps, session recordings, and behavioral analytics that reveal UX insights.

## Description
Connect your **Microsoft Clarity** account to any AI agent and unlock behavioral analytics insights through natural conversation.

### What you can do

- **Project Management** — List all tracked websites and inspect individual project configurations and data retention settings
- **Live Insights** — Retrieve real-time active users, page views, and engagement metrics for any project
- **Dashboard Analytics** — Access aggregate metrics including sessions, pages per session, engagement scores, and bounce rates
- **Heatmap Analysis** — Browse page heatmaps showing click, scroll, and attention patterns, and inspect detailed interaction data
- **Session Recordings** — List session recordings with duration and pages visited, and inspect individual session timelines
- **UX Friction Detection** — Identify dead clicks (elements that don't respond) and rage clicks (repeated frustrated clicking) to locate broken UI elements
- **Content Visibility** — Analyze scroll depth data to understand how far users scroll and where content engagement drops off
- **Page Ranking** — View top-performing pages ranked by session count and engagement metrics

### How it works

1. Subscribe to this server
2. Enter your Clarity API Key
3. Start analyzing user behavior from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UX Designers** — identify friction points, analyze click patterns, and validate design decisions with behavioral data
- **Product Managers** — monitor engagement metrics, track feature adoption through scroll depth, and prioritize UX improvements
- **Growth Engineers** — detect conversion blockers by analyzing rage clicks, dead clicks, and session replay data


## Available Tools (13)
- **check_clarity_status**: Verify connectivity
- **get_dashboard**: Get dashboard metrics
- **get_heatmap**: Get heatmap data
- **get_live_insights**: Get live insights
- **get_project**: Get project details
- **get_recording**: Get recording details
- **get_scroll_depth**: Get scroll depth
- **list_dead_clicks**: List dead clicks
- **list_heatmaps**: List heatmaps
- **list_projects**: List projects
- **list_rage_clicks**: List rage clicks
- **list_recordings**: List recordings
- **list_top_pages**: List top pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft Clarity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all rage clicks and dead clicks on our checkout page this week."

**🤖 AI Agent:**
> Analyzing project 'E-commerce Site' (proj_501)... Found 34 rage click events on the checkout page. The hotspot is the 'Apply Coupon' button (89% of rage clicks) — users are clicking repeatedly because the button takes 4+ seconds to respond. Dead clicks: 12 events on the 'Shipping Options' section — the estimated delivery dates look clickable but aren't interactive. Would you like to see the heatmap or session recordings for this page?

---

**👤 You:**
> "What are the top 5 most visited pages and how far do users scroll on the homepage?"

**🤖 AI Agent:**
> Top 5 pages by sessions: 1) Homepage — 28,400 sessions, 3.2 engagement score. 2) /pricing — 12,100 sessions, 4.1 engagement. 3) /features — 8,900 sessions. 4) /checkout — 6,200 sessions. 5) /blog — 5,800 sessions. Scroll depth for Homepage: 100% reach the hero section, 78% reach the features grid, 52% reach testimonials, 31% reach the footer CTA. Content below the fold has a 48% drop-off. Would you like to see the heatmap?

---

**👤 You:**
> "How many active users are on the site right now and what pages are they viewing?"

**🤖 AI Agent:**
> Live insights for 'E-commerce Site' (proj_501): 142 active users right now. Top pages being viewed: /pricing (34 users), Homepage (28 users), /features (19 users), /checkout (15 users), /blog/ai-tools-2025 (12 users). Average session duration: 4m 12s. Engagement score (live): 3.8/5. Traffic is 23% higher than the same time yesterday. Would you like to see the dashboard metrics for the full day?


## ❓ FAQ

**Q: Can I detect UX friction points like dead clicks and rage clicks?**
Yes! Use `list_dead_clicks` to find page elements where users click without any response — signaling non-interactive elements that look clickable. Use `list_rage_clicks` to detect pages where users repeatedly click in frustration, indicating broken buttons, slow-loading elements, or confusing UI patterns.

**Q: Can I analyze how far users scroll on each page?**
Yes. The `get_scroll_depth` tool returns scroll metrics for each page in your project, showing the percentage of users who reach each content section. This identifies exactly where engagement drops off — essential for optimizing content placement and CTA positioning.

**Q: Can I view real-time analytics while users are on my site?**
Yes. The `get_live_insights` tool provides real-time data for any project, including active user count, current page views, and live engagement metrics. For historical aggregates, use `get_dashboard` to access sessions, pages per session, and engagement scores over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-clarity](https://vinkius.com/mcp/microsoft-clarity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft Clarity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microsoft-clarity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft Clarity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-clarity": {
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
