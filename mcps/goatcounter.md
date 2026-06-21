# GoatCounter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goatcounter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Privacy-friendly web analytics — track pageviews, analyze visitor stats, and manage your sites directly through any AI agent.

## Description
Connect your **GoatCounter** account to any AI agent to monitor your web traffic without compromising user privacy. This MCP server allows you to query detailed statistics, manage site configurations, and handle data exports through natural conversation.

### What you can do

- **Traffic Insights** — Retrieve pageview counts, total hits, and referral statistics for specific paths.
- **Visitor Analytics** — Break down stats by categories such as browsers, operating systems, locations, and languages.
- **Data Portability** — Initiate, monitor, and download full CSV/JSON data exports for external analysis.
- **Site Management** — List all your registered sites, create new ones, or update existing site configurations.
- **Custom Event Tracking** — Send hits or events directly from your backend or middleware to your GoatCounter dashboard.

### How it works

1. Subscribe to this server
2. Enter your GoatCounter API Key and your instance URL
3. Start analyzing your web traffic from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — monitor site performance and visitor trends without leaving the code editor.
- **Data Analysts** — automate the extraction of privacy-compliant analytics for custom reporting.
- **Site Owners** — get quick summaries of daily traffic and top-performing content via simple chat commands.


## Available Tools
- **count_hits**: Send pageviews or events to GoatCounter
- **create_site**: Create a new site
- **download_export**: Download a completed export file
- **get_export**: Get export status and metadata
- **get_site**: Detailed information about a site
- **list_sites**: List all sites accessible by the user
- **get_me**: Get current user and API key info
- **start_export**: Returns an export ID to check status.

Start a new data export in the background
- **get_stats_hits_path**: Referral statistics for a specific path
- **get_stats_hits**: Overview of pageviews per path
- **get_stats_page_detail**: g., browser versions).

Detailed stats for a specific item in a category
- **get_stats_page**: Stats for specific categories (browsers, systems, etc)
- **get_stats_total**: Total pageview counts for a date range
- **update_site**: Update site settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoatCounter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the total pageview counts for the last 30 days."

**🤖 AI Agent:**
> I've retrieved your stats. In the last 30 days, your site received a total of 12,450 pageviews.

---

**👤 You:**
> "List all the sites registered in my GoatCounter account."

**🤖 AI Agent:**
> You have 3 sites registered: 'Personal Blog' (ID: 101), 'E-commerce Store' (ID: 102), and 'Docs Portal' (ID: 103).

---

**👤 You:**
> "Get detailed stats for browser versions used by my visitors."

**🤖 AI Agent:**
> Analyzing browser data... Chrome 118 is your most popular version (45%), followed by Firefox 119 (20%) and Safari 17 (15%).


## ❓ FAQ

**Q: Can I see which browsers my visitors are using?**
Yes. Use the `get_stats_page` tool with the 'browsers' category to see a breakdown of visitor browser statistics for your chosen date range.

**Q: How do I export all my analytics data for backup?**
You can start a background export using `start_export`. Once processed, use `get_export` to check the status and `download_export` to retrieve the file.

**Q: Is it possible to track custom events from my server code?**
Absolutely. The `count_hits` tool allows you to send pageviews or custom events directly to GoatCounter from any backend or middleware.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goatcounter](https://vinkius.com/mcp/goatcounter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoatCounter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `goatcounter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoatCounter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goatcounter": {
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
