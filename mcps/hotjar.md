# Hotjar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hotjar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Understand your users with heatmaps, session recordings, and feedback surveys that reveal exactly why visitors leave your site.

## Description
Connect your **Hotjar** account to any AI agent and access user experience analytics through natural conversation.

### What you can do

- **Survey Management** — List all surveys, inspect questions and settings, retrieve individual responses, and review aggregate statistics (completion rate, NPS score, trends)
- **Feedback Widgets** — Browse incoming feedback widgets, inspect rating breakdowns, and review individual user submissions with screenshots
- **Heatmaps** — List all heatmap snapshots and inspect click, scroll, and move data for specific pages
- **Session Recordings** — Browse session recordings with duration and page count, and inspect metadata and events for individual sessions
- **Conversion Funnels** — List all funnels with step-by-step drop-off data for conversion optimization
- **User Lookup** — Retrieve session history and behavior data for a specific user ID
- **Site Management** — List all tracked sites configured in your Hotjar account

### How it works

1. Subscribe to this server
2. Enter your Hotjar Client Secret from the API settings
3. Start analyzing user behavior from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UX Researchers** — review survey responses, analyze heatmap patterns, and watch session recordings to understand user behavior
- **Product Managers** — track conversion funnels, identify drop-off points, and monitor NPS scores
- **Growth Teams** — analyze feedback trends, optimize page engagement, and identify usability issues through AI


## Available Tools
- **check_hotjar_status**: Verify connectivity
- **get_feedback_widget**: Get feedback widget details
- **get_heatmap**: Get heatmap details
- **get_recording**: Get recording details
- **get_survey_stats**: Get survey statistics
- **get_survey**: Get survey details
- **list_feedback_responses**: List feedback responses
- **list_feedback**: List feedback widgets
- **list_funnels**: List funnels
- **list_heatmaps**: List heatmaps
- **list_recordings**: List recordings
- **list_sites**: List tracked sites
- **list_survey_responses**: List survey responses
- **list_surveys**: List surveys
- **lookup_user**: Lookup user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotjar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the NPS survey results and the top feedback submissions this month."

**🤖 AI Agent:**
> NPS Survey 'Product Satisfaction Q2' (survey_401): NPS Score: 42 (Good). Promoters: 58%, Passives: 26%, Detractors: 16%. Completion rate: 34.2% (342 responses / 1,000 views). Response trend: +8% vs last month. Top feedback submissions: 1) ⭐⭐⭐⭐⭐ 'Love the new dashboard redesign!' — /dashboard page. 2) ⭐⭐ 'Checkout is too slow on mobile' — /checkout (screenshot attached). 3) ⭐⭐⭐⭐ 'Would be great to have dark mode' — /settings. 4) ⭐ 'Can't find the export button' — /reports. Would you like to see the heatmap for the checkout page or the full survey responses?

---

**👤 You:**
> "Show the heatmap data for our pricing page and the conversion funnel from landing to signup."

**🤖 AI Agent:**
> Pricing page heatmap (heatmap_089): Click data: 'Pro Plan CTA' button — 342 clicks (hottest). 'Compare Plans' toggle — 189 clicks. 'Enterprise Contact' link — 67 clicks. FAQ accordion — 45 clicks. Scroll data: 78% of users scroll past the hero section. Only 34% reach the FAQ section at bottom. Conversion funnel 'Landing → Signup': Step 1: Landing page — 8,400 visitors (100%). Step 2: Pricing page — 3,200 (38.1%, -61.9% drop). Step 3: Plan selection — 1,100 (34.4%, -65.6% drop). Step 4: Signup form — 680 (61.8%, -38.2% drop). Step 5: Completed signup — 420 (61.8% of form, 5% overall). Biggest drop-off: Landing → Pricing (61.9%). Would you like to see session recordings from the pricing page?

---

**👤 You:**
> "Look up user behavior for user ID 'usr_12345' and show their session recordings."

**🤖 AI Agent:**
> User 'usr_12345': 7 sessions over 3 weeks. Device: Chrome/Desktop (5 sessions), Safari/Mobile (2). Total time on site: 48 minutes. Pages viewed: 23. Key behaviors: Visited /pricing 4 times but never clicked a CTA. Spent 8 minutes on /features reading comparison table. Submitted feedback: 'Pricing is confusing' (2 stars). Session recordings: 1) rec_7701 (Apr 20, 12 min, 6 pages — desktop). 2) rec_7689 (Apr 15, 8 min, 4 pages). 3) rec_7645 (Apr 10, 5 min, 3 pages — mobile). This user shows high interest but pricing friction. Would you like to watch a specific recording?


## ❓ FAQ

**Q: Can I view survey responses and NPS scores?**
Yes. Use `list_surveys` to see all surveys with response counts and status. Use `get_survey_stats` for aggregate metrics including completion rate, NPS score, and response trends. Use `list_survey_responses` to read individual user responses. Use `get_survey` for the full question list and settings.

**Q: Can I analyze heatmap data for specific pages?**
Yes. Use `list_heatmaps` to browse all heatmap snapshots, then `get_heatmap` with a specific Heatmap ID to retrieve click, scroll, and move interaction data along with the page URL. This reveals where users focus attention and which elements they interact with most.

**Q: Can I track conversion funnel drop-offs?**
Yes. The `list_funnels` tool retrieves all configured conversion funnels with step-by-step drop-off data. Each funnel shows the number of users entering each step and the percentage that continue to the next, helping you identify exactly where users abandon the flow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hotjar](https://vinkius.com/mcp/hotjar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotjar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hotjar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotjar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotjar": {
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
