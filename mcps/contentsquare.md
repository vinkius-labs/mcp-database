# Contentsquare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentsquare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage UX analytics via Contentsquare — track site metrics, list demographic segments, audit URL mappings, and export raw data directly from any AI agent.

## Description
Connect your **Contentsquare** account to any AI agent and take full control of your digital experience analytics and UX monitoring through natural conversation.

### What you can do

- **Project & Metric Auditing** — List project directories and retrieve explicit site metrics including bounce rates, engagement, and conversion telemetry
- **Audience Segmentation** — Access standard API demographic directories to classify user behaviors and validate platform segments globally
- **URL & Zoning Analysis** — Discover explicit routing trees for URL paths and inspect deep interaction arrays like heatmap coordinates and button zones
- **Raw Data Exports** — Trigger automated raw data pipeline extractions for sessions or pageviews to feed your external BI tools or data science workflows
- **Session Enrichment** — Mutate global boundaries by appending offline attributes (like sales or contact logs) to live active interaction blocks
- **Page-Level Deep Dives** — Execute direct queries for specific document nodes to track detailed behavioral limits against exact page URLs

### How it works

1. Subscribe to this server
2. Enter your Contentsquare Client ID, Client Secret, and Project ID (Found in the Contentsquare Console under API Credentials)
3. Start auditing your digital experience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UX Researchers** — audit user behavior metrics and heatmap zonings without digging through the full console
- **Product Managers** — monitor project-wide engagement and conversion trends using natural language
- **Data Analysts** — trigger raw data exports and enrich sessions with offline data directly from the chat
- **Digital Marketers** — verify audience segment behavior and audit page-level performance for specific campaigns


## Available Tools (10)
- **list_projects**: Identify bounded UX tracking domains inside the Headless Contentsquare platform
- **get_metrics**: Retrieve explicit UX logging tracing explicit bounce / engagement metrics
- **list_segments**: Provision highly-available JSON arrays holding demographic limits
- **list_mappings**: Discover explicit routing trees structuring specific URL paths
- **list_zonings**: Inspect deep internal interaction arrays mitigating specific Click tracking constraints
- **create_export_job**: Dispatch an automated validation check routing Raw Data Pipeline chunks
- **get_export_job**: Validate Data Science object extraction execution state queues
- **list_export_jobs**: Perform structural log extraction matching asynchronous Raw export payloads
- **get_page_metrics**: Execute static generation targeting exactly formatted URL statistical bodies
- **enrich_session**: g. Sales, Contact logs) binding native JSON payloads executing directly towards session arrays.

Mutate global Web CRM boundaries appending headless Offline attributes to live sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contentsquare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Contentsquare"

**🤖 AI Agent:**
> I found 3 active projects: 'Main Website (ID: 123)', 'Mobile App (ID: 456)', and 'Staging Site (ID: 789)'. Which one would you like to audit for metrics?

---

**👤 You:**
> "Get site metrics for last week"

**🤖 AI Agent:**
> Retrieving metrics for Jan 1st - Jan 7th... Site Engagement: 65%, Bounce Rate: 32%, Conversion Rate: 4.5%. Performance is stable compared to the previous week.

---

**👤 You:**
> "Create a raw data export for sessions from yesterday"

**🤖 AI Agent:**
> Export job initiated! Job ID: 'export_abc123'. Contentsquare is now processing the raw session chunks for yesterday. I can check the status for you in a few minutes.


## ❓ FAQ

**Q: Can my agent export raw session data from Contentsquare?**
Yes. Use the 'create_export_job' tool with your desired date range and data type (sessions or pageviews). The agent will initiate the asynchronous extraction and provide you with a job ID to monitor the download status.

**Q: How do I enrich an active session with offline sales data?**
Provide the session ID and a JSON object containing the properties you want to append. The 'enrich_session' tool will push these attributes directly to the active interaction block within the Contentsquare engine.

**Q: Can I check the engagement metrics for a specific landing page URL?**
Absolutely. Use the 'get_page_metrics' tool. Provide the exact page URL and a date range. Your agent will return detailed statistical bodies including bounce rates and behavioral limits for that specific web document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentsquare](https://vinkius.com/mcp/contentsquare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contentsquare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contentsquare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contentsquare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contentsquare": {
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
