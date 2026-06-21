# GoSquared MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gosquared)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Monitor real-time web traffic and analyze historical trends via AI.

## Description
Connect your **GoSquared** account to your AI agent and get instant, conversational access to your web analytics. Query real-time active visitors, track marketing campaign performance, and analyze historical traffic trends directly from your workflow.

### What you can do

- **Real-Time Analytics (Now API)** — Check exactly how many visitors are on your site right now, what pages they are viewing, and where they came from
- **Historical Trends (Trends API)** — Analyze past traffic data, including page views, traffic sources, and campaign effectiveness over specific date ranges
- **Audience Insights** — Understand your visitors' technology preferences with detailed breakdowns of browsers and devices

### How it works

1. Subscribe to this server
2. Enter your GoSquared Site Token and API Key (found in your account settings)
3. Start querying your web analytics from Claude, Cursor, or any MCP-compatible client

Your AI agent acts as a dedicated web analyst, transforming complex dashboards into simple, actionable answers.

### Who is this for?

- **Marketing Teams** — instantly check how much live traffic a new campaign or newsletter is generating
- **Product Managers** — analyze historical page view trends to understand feature adoption and user behavior
- **Website Owners** — keep a pulse on your site's performance without constantly logging into an analytics dashboard


## Available Tools
- **get_now_campaigns**: Get active campaigns currently driving traffic
- **get_now_overview**: Get a top-level overview of concurrent active visitors
- **get_now_pages**: Get a list of pages currently being viewed
- **get_now_sources**: Get active traffic sources (referrers)
- **get_now_visitors**: Get a list of individual visitors currently online
- **get_trends_browsers**: Get historical browser breakdown data
- **get_trends_campaigns**: Get historical campaign performance data
- **get_trends_devices**: Get historical device breakdown data
- **get_trends_overview**: Get historical aggregate data overview
- **get_trends_pages**: Get historical aggregate data for pages
- **get_trends_sources**: Get historical traffic sources data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoSquared** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many visitors are on the site right now?"

**🤖 AI Agent:**
> Checking real-time analytics... You currently have 142 active visitors on your site. 85 of them are actively engaging with the content.

---

**👤 You:**
> "What were our top traffic sources yesterday?"

**🤖 AI Agent:**
> Retrieving trends... Yesterday, your top traffic sources were:
1. Google (Organic): 1,200 visits
2. Direct: 850 visits
3. Twitter / X: 420 visits
4. LinkedIn: 150 visits

---

**👤 You:**
> "Tell me what percentage of visitors today are using mobile phones."

**🤖 AI Agent:**
> Checking technology insights... So far today, 62% of your site traffic is originating from mobile devices, predominantly iOS.


## ❓ FAQ

**Q: Can I see exactly how many people are on my site right now?**
Yes! The `get_now_overview` tool provides an instant snapshot of your concurrent active visitors. You can also use `get_now_pages` to see exactly which URLs they are currently reading.

**Q: How do I check traffic for a specific day in the past?**
You can use any of the `get_trends_*` tools (like `get_trends_overview`) and provide the `date` parameter. You can use 'today', 'yesterday', or a specific date format like 'YYYY-MM-DD'.

**Q: Does it track which external links visitors click?**
Yes. The real-time events functionality tracks specific outbound interactions out of the box, exposing exactly what resources capture audience interest the most.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gosquared](https://vinkius.com/mcp/gosquared)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoSquared** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gosquared` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoSquared** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gosquared": {
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
