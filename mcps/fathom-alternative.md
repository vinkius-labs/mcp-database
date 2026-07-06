# Fathom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fathom-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Privacy-first website analytics — track visitors, monitor real-time traffic, and manage sites and events directly from your AI agent.

## Description
Connect your **Fathom Analytics** account to any AI agent to monitor your website performance while respecting user privacy. Get instant access to traffic data, site management, and event tracking through natural conversation.

### What you can do

- **Real-time Monitoring** — Check exactly how many visitors are on your site right now with live data.
- **Analytics Aggregations** — Retrieve complex data aggregations for pageviews, uniques, and bounce rates across specific timeframes.
- **Site Management** — List, create, update, or delete sites in your Fathom account without leaving your workflow.
- **Event & Milestone Tracking** — Monitor specific conversions, list active events, and manage milestones to track your business goals.
- **Account Overview** — Quickly retrieve account details and owner information associated with your API token.

### How it works

1. Subscribe to this server
2. Enter your Fathom API Token
3. Start querying your analytics from Claude, Cursor, or any MCP-compatible client

No more digging through dashboards to find simple traffic stats. Your AI acts as a data analyst that respects privacy laws by default.

### Who is this for?

- **Digital Marketers** — instantly check campaign performance and event completion rates.
- **Site Owners** — monitor real-time traffic spikes and site health directly from a chat interface.
- **Developers** — manage site configurations and event IDs straight from the code editor.


## Available Tools (20)
- **get_aggregations**: Generate flexible reports by grouping and filtering data
- **create_site**: Create a new Fathom site
- **get_current_visitors**: Returns the total current visitors on a site
- **delete_event**: Permanently delete an event
- **delete_milestone**: Permanently delete a milestone
- **delete_site**: Permanently delete a site
- **get_event**: Retrieve a single event by its ID
- **get_milestone**: Retrieve a single milestone by its ID
- **get_site**: Retrieve a single site by its ID
- **list_events**: List all events for a site
- **list_milestones**: List all milestones for a site
- **list_sites**: Supports cursor pagination.

List all sites owned by the API key
- **update_event**: Update an existing event
- **update_milestone**: Update an existing milestone
- **update_site**: Update an existing Fathom site
- **wipe_event**: Wipe all completion data for an event
- **wipe_site**: Wipe all pageviews and event completions from a site
- **get_account**: Retrieve information about the Fathom account owner
- **create_event**: Create a new event for a site
- **create_milestone**: Create a new milestone for a site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fathom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many visitors are currently on my site with ID CNDY123?"

**🤖 AI Agent:**
> Checking real-time data... There are currently 42 active visitors on your site (ID: CNDY123).

---

**👤 You:**
> "List all the sites in my Fathom account."

**🤖 AI Agent:**
> I've retrieved your sites. You have 3 sites: 'Personal Blog' (ID: BLOG1), 'E-commerce Store' (ID: SHOP2), and 'Portfolio' (ID: PORT3).

---

**👤 You:**
> "Get the pageviews and unique visitors for site SHOP2 for the last 7 days."

**🤖 AI Agent:**
> Fetching aggregations... For the last 7 days, site SHOP2 had 1,250 pageviews and 890 unique visitors.


## ❓ FAQ

**Q: Can I see how many people are on my website right now?**
Yes! Use the `getCurrentVisitors` tool with your Site ID to get the current number of active visitors on your website in real-time.

**Q: How do I get a summary of my traffic for a specific period?**
You can use the `get_aggregations` tool. It allows you to specify metrics like `pageviews` or `uniques` and define time filters to get summarized data.

**Q: Can I manage my site settings through this integration?**
Absolutely. You can use `list_sites` to see all your sites, `create_site` to add new ones, and `update_site` to change names or sharing preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fathom-alternative](https://vinkius.com/mcp/fathom-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fathom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fathom-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fathom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fathom-alternative": {
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
