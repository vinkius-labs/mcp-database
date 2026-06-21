# Umami Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/umami-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Privacy-focused web analytics alternative to Google Analytics.

## Description
The Umami Cloud MCP Server connects AI agents to the Umami Analytics API. It allows agents to retrieve real-time and historical website statistics, fetch pageviews, analyze active users, and export events dynamically while preserving end-user privacy.


## Available Tools
- **users**: Get the number of active users on a website
- **websites**: Get specific metrics (urls, browsers, os, devices) for a website


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Umami Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 pages by pageviews on my main website for the last 7 days."

**🤖 AI Agent:**
> Here are the top pages: 1. /home (5,000 views), 2. /pricing (1,200 views)...

---

**👤 You:**
> "Analyze the bounce rate and absolute session duration from mobile users on the pricing page today."

**🤖 AI Agent:**
> Fetching Umami metrics ('get_page_metrics')...
Mobile Traffic (URL: `/pricing` - Today):
- Unique Visitors: 1,840 
- Bounce Rate: 54.2%
- Average Session Duration: 1m 42s

---

**👤 You:**
> "List the top 4 referral traffic sources matching 'social' for this month."

**🤖 AI Agent:**
> Querying referral patterns on Umami Cloud ('get_referrers')...
Top 'Social' Referrers:
1. Twitter/X: 4,112 visits
2. LinkedIn: 2,890 visits
3. HackerNews: 1,140 visits
4. Reddit: 885 visits


## ❓ FAQ

**Q: What data can AI generate from Umami Cloud?**
AI can query active users individually, metrics by website, page view breakdowns, browser/OS statistics, and custom triggered events.

**Q: How does the MCP authenticate with Umami Cloud?**
The integration uses an API access token. Provide your Umami Cloud token manually or pass username and password.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umami-cloud](https://vinkius.com/mcp/umami-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Umami Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `umami-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Umami Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "umami-cloud": {
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
