# Klipfolio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klipfolio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Build real-time business dashboards that pull from hundreds of data sources and give every stakeholder the metrics they need.

## Description
Connect your **Klipfolio** account to any AI agent and manage analytics dashboards through natural conversation.

### What you can do

- **Dashboard Browsing** — List all dashboards and inspect their layouts
- **Klip Management** — Browse individual Klips (widgets) with their data and configurations
- **Data Sources** — List connected data sources and their refresh status
- **KPI Monitoring** — Access real-time metrics and key performance indicators

### How it works

1. Subscribe to this server
2. Enter your Klipfolio API Key
3. Start browsing analytics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Executives** — view KPIs and dashboards without opening the app
- **Analytics Teams** — monitor data source health and refresh status
- **Marketing** — check campaign metrics and performance Klips


## Available Tools (6)
- **list_individual_klips**: List all individual Klips
- **list_account_clients**: List sub-clients
- **list_dashboards**: List Klipfolio dashboards
- **list_data_sources**: List data source instances
- **get_dashboard_details**: Get details for a specific dashboard
- **refresh_data_source**: Trigger data source refresh


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klipfolio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all dashboards and the KPIs on the Executive Dashboard."

**🤖 AI Agent:**
> Dashboards: 5. Executive Overview (8 Klips), Marketing Performance (12), Sales Pipeline (6), Engineering Metrics (4), Customer Success (5). Executive Klips: MRR ($125K, +8% MoM), ARR ($1.5M), Active Users (12.4K, +3%), Churn Rate (2.1%), NPS (72), CAC ($145), LTV ($2,100), Revenue Growth (+18% YoY).

---

**👤 You:**
> "List data sources and check if any are failing."

**🤖 AI Agent:**
> Data sources: 8. ✅ Google Analytics (refreshed 5 min ago). ✅ Stripe (refreshed 2 min ago). ✅ HubSpot (refreshed 10 min ago). ✅ Salesforce (refreshed 15 min ago). ⚠️ PostgreSQL (stale, last refresh 2h ago). ✅ Intercom (refreshed 8 min ago). ❌ Facebook Ads (auth expired, failed 1h ago). ✅ Mixpanel (refreshed 12 min ago). Action needed: Reconnect Facebook Ads, investigate PostgreSQL.

---

**👤 You:**
> "Show the Marketing Performance dashboard Klips."

**🤖 AI Agent:**
> Marketing Performance: 12 Klips. Email: Open Rate (29%), Click Rate (6.4%), Subscribers (45K). Ads: CPC ($1.24), CTR (3.8%), ROAS (4.2x). Social: Followers (28K, +2.1K/mo), Engagement (5.2%). Website: Sessions (125K/mo), Bounce Rate (42%), Conversion (3.1%). Budget: $45K spent / $50K allocated.


## ❓ FAQ

**Q: Can I view dashboards and KPIs through the AI agent?**
Yes. List all dashboards, browse individual Klips with their current data values, and monitor KPIs in real-time.

**Q: Can I check data source health?**
Yes. List all connected data sources with their last refresh time, status, and error details when applicable.

**Q: What API endpoint does Klipfolio use?**
Klipfolio uses proprietary API Key authentication via the `kf-api-key` header against `api.klipfolio.com/api/1.0`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klipfolio](https://vinkius.com/mcp/klipfolio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Klipfolio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klipfolio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Klipfolio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klipfolio": {
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
