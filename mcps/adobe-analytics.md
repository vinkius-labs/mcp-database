# Adobe Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adobe-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Customer journey insights — retrieve reports, manage segments, and audit metrics via AI.

## Description
Connect your **Adobe Analytics** account to your AI agent to unlock deep customer journey insights and real-time data orchestration. From retrieving complex reporting breakdowns to managing audience segments and auditing calculated metrics, your agent handles your enterprise analytics ecosystem through natural conversation.

### What you can do

- **Enterprise Reporting** — Retrieve synchronous reports with nested breakdowns and complex filters directly from chat
- **Component Discovery** — List and audit all available metrics and dimensions for your specific report suites
- **Segment Management** — List and retrieve details for audience segments to ensure your data is always relevant
- **Report Suite Oversight** — Manage and list your report suites (collections) to maintain organizational control
- **Real-time Performance** — Quickly identify traffic trends and engagement patterns without manual dashboard configuration

### How it works

1. Subscribe to this server
2. Enter your Adobe Client ID, Client Secret, and Global Company ID
3. Start managing your enterprise analytics and retrieving insights through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — automate report retrieval and technical metadata audits effortlessly
- **Marketing Managers** — monitor campaign performance and segment engagement on the fly
- **Growth Leads** — verify conversion trends and identification patterns across multiple report suites
- **Product Owners** — retrieve feature engagement data and user journey patterns using simple commands


## Available Tools
- **list_report_suites**: List available report suites
- **get_metrics**: List metrics for a report suite
- **get_dimensions**: g. Page, Device Type) for a specific report suite ID.

List dimensions for a report suite
- **get_report**: 0 JSON report request body.

Retrieve an analytics report
- **list_segments**: List audience segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adobe Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all metrics available for report suite 'mycompany-prod'."

**🤖 AI Agent:**
> I've retrieved the metrics for 'mycompany-prod'. You have 50 standard metrics (like Page Views, Visits) and 12 calculated metrics (like Conversion Rate) available.

---

**👤 You:**
> "Show me the top 5 pages by visits for yesterday."

**🤖 AI Agent:**
> I've generated the report. Yesterday's top pages were: 1. Home, 2. Product Catalog, 3. Checkout, 4. About Us, 5. Blog. Would you like to see the bounce rate for these pages?

---

**👤 You:**
> "List all active segments in my Adobe Analytics account."

**🤖 AI Agent:**
> I've retrieved your segments. You have 25 active segments, including 'Mobile Users', 'Purchasers', and 'New Visitors'. Would you like to see the definition for a specific segment?


## ❓ FAQ

**Q: Where do I find my Global Company ID?**
The easiest way is to log in to the Adobe Developer Console and check your project settings. Alternatively, once you have an access token, the `list_report_suites` tool will return your authorized company metadata.

**Q: Are reports returned in real-time?**
Yes. Unlike older versions of the API, the v2.0 Reporting API is synchronous and returns the data directly in the request response, making it perfect for AI interactions.

**Q: Does this support complex breakdowns?**
Yes, the `get_report` tool accepts a JSON payload that supports the full range of Adobe Analytics v2.0 reporting features, including nested breakdowns and metric filters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adobe-analytics](https://vinkius.com/mcp/adobe-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adobe Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adobe-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adobe Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adobe-analytics": {
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
