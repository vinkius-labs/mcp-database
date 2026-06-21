# Octoboard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/octoboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build client-facing marketing reports automatically by pulling data from Google, Facebook, HubSpot, and 50 other integrations.

## Description
Connect your **Octoboard** account to any AI agent and take full control of your marketing business intelligence and reporting orchestration through natural conversation. Octoboard provides a powerful data visualization platform, and this integration allows you to retrieve dashboard metadata, push custom metrics to widgets, and monitor automated reports directly from your chat interface.

### What you can do

- **Dashboard & Report Orchestration** — List all active dashboards and retrieve detailed report metadata programmatically to ensure your team's visual insights are always synchronized.
- **Custom Data Intelligence** — Push numeric, text, or status metrics directly into Octoboard widgets from the AI interface to maintain real-time tracking of proprietary data.
- **Visual Data Control** — Send bar chart arrays, data tables, and variation metrics via natural language to drive better data transparency across your organization.
- **Agency & Client Oversight** — List managed clients and monitor account usage using simple AI commands to maintain a clear overview of your digital agency operations.
- **Operational Monitoring** — Track system responses and manage API health to ensure your reporting pipelines are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Octoboard API Key from your account settings
3. Start managing your marketing metrics from Claude, Cursor, or any MCP-compatible client

No more manual data entry into reporting tools. Your AI acts as a dedicated data analyst or business intelligence coordinator.

### Who is this for?

- **Marketing Agencies** — quickly update custom client metrics and monitor dashboard health without switching apps.
- **Data Analysts** — automate the pushing of proprietary business data and track report delivery via natural conversation.
- **Business Owners** — streamline the retrieval of high-level revenue metrics and monitor organizational growth directly within the chat.


## Available Tools (12)
- **get_api_status**: Check connection
- **check_api_usage**: Check data limits
- **list_agency_clients**: List managed clients
- **list_active_dashboards**: List dashboards
- **list_automated_reports**: List reports
- **push_bar_chart**: Update bar chart
- **push_numeric_metric**: Update widget number
- **push_status_update**: Update status indicator
- **push_data_table**: Update data table
- **push_text_metric**: Update widget text
- **push_variation_metric**: g. 10.5) to a widget.

Update value + change
- **test_octoboard_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Octoboard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active dashboards in Octoboard."

**🤖 AI Agent:**
> I've retrieved your dashboards. You have 3 active environments: 'Client A - Marketing', 'Internal Revenue', and 'SEO Performance'. Which one would you like to see metrics for?

---

**👤 You:**
> "Push a revenue metric of 48750 to my Executive KPI dashboard widget."

**🤖 AI Agent:**
> Done. The numeric metric $48,750 has been pushed to your Executive KPI dashboard. The widget now displays the updated value with a 12% increase indicator compared to the previous period. The dashboard will refresh for all viewers within 30 seconds.

---

**👤 You:**
> "List all automated reports and their delivery schedules."

**🤖 AI Agent:**
> You have 4 automated reports configured. "Weekly SEO Summary" sends every Monday at 9 AM to marketing@company.com. "Monthly Client Report" generates the 1st of each month for 6 agency clients. "Daily Ad Spend" delivers at 8 AM to the growth team. "Quarterly Executive Review" runs every quarter end.


## ❓ FAQ

**Q: Can my AI automatically find the Widget ID for a custom data widget?**
The Widget ID is found in the Octoboard dashboard settings for any 'Custom Data' widget. You must provide this ID when using the `send_numeric_metric` or similar tools.

**Q: How do I find my Octoboard API Key?**
Log in to Octoboard, navigate to your **Account Settings** > **API**, and you will find your unique secret token there.

**Q: Can I push table data to Octoboard using the AI?**
Yes! Use the `send_table_data` tool. Provide the Widget ID, headers, and a 2D array of rows, and your agent will update the corresponding data table widget instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/octoboard](https://vinkius.com/mcp/octoboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Octoboard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `octoboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Octoboard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "octoboard": {
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
