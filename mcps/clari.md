# Clari MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clari)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage revenue intelligence and forecasting via Clari — track opportunities, monitor forecasts, and audit pipeline changes directly from any AI agent.

## Description
Connect your **Clari** account to any AI agent and take full control of your revenue operations and forecasting through natural conversation. Streamline how you manage your sales pipeline and historical revenue data.

### What you can do

- **Opportunity Oversight** — List and retrieve details for all CRM opportunities tracked in Clari natively
- **Forecast Intelligence** — Access manual forecast submissions and historical data to understand trends flawlessly
- **Pipeline Auditing** — List and review platform events and audit trail records to track changes securely
- **Account Visibility** — Access CRM accounts associated with revenue data and monitor their status flawlessly
- **User Logistics** — List all users and organization hierarchies to understand team performance securely
- **Export Intelligence** — Monitor the status of asynchronous bulk data export jobs directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clari API Token (obtained from Settings or Clari Support)
3. Start managing your revenue intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Leaders** — monitor forecast accuracy and pipeline health using natural language
- **Revenue Operations** — audit changes to opportunities and monitor export job statuses without opening the dashboard
- **Account Executives** — quickly look up opportunity details and historical forecast values straight from their chat interface
- **Finance Teams** — verify revenue snapshots and fiscal time period configurations


## Available Tools (8)
- **list_clari_users**: List all users and hierarchy in the account
- **get_opportunity_revenue_details**: Get detailed information for a specific opportunity
- **list_revenue_accounts**: List CRM accounts associated with revenue data
- **list_clari_audit_logs**: List platform events and audit trail records
- **list_clari_export_jobs**: List status of asynchronous bulk data export jobs
- **list_clari_forecasts**: List manual forecast submissions and historical data
- **list_revenue_opportunities**: List CRM opportunities tracked in Clari
- **list_clari_time_periods**: List active fiscal years, quarters, and months used in Clari


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clari** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all opportunities worth over $50,000."

**🤖 AI Agent:**
> Retrieving your high-value opportunities... I found 3 deals: 'Acme Enterprise Expansion' ($120k), 'Global Logistics Q3' ($75k), and 'TechCorp Pilot' ($55k). Would you like the full details for the Acme deal?

---

**👤 You:**
> "What is our current manual forecast value?"

**🤖 AI Agent:**
> Checking latest forecast submissions... For the current quarter, the manual aggregate forecast is $2.4M across all regions. This is a 10% increase compared to last week's snapshot.

---

**👤 You:**
> "Who are the account owners for the 'Top 10' pipeline accounts?"

**🤖 AI Agent:**
> Retrieving account ownership data... The Top 10 accounts are managed by: Sarah Miller (4 accounts), Mike Scott (3 accounts), and John Doe (3 accounts).


## ❓ FAQ

**Q: Can I see my team's forecast for this quarter?**
Yes! Use the `list_clari_forecasts` tool. The agent will return the latest forecast submissions and historical values, allowing you to see the projected revenue for the current fiscal period.

**Q: How do I check for recent changes in a specific opportunity?**
Use the `list_clari_audit_logs` tool. Your agent will fetch the platform's audit trail, which includes updates to opportunity stages, amounts, and other key revenue metrics.

**Q: Where do I find my Clari API Token?**
Clari API tokens are typically provided through your Clari Settings page. If you don't see the API section, you may need to contact your Clari account manager or support team to enable Export API access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clari](https://vinkius.com/mcp/clari)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clari** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clari` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clari** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clari": {
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
