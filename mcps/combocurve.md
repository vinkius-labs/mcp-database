# ComboCurve MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/combocurve)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Enable your AI agent to manage wells, projects, and production forecasts via the ComboCurve API.

## Description
Connect your AI assistant to **ComboCurve**, the cloud-based energy platform for forecasting, valuation, and reporting in the oil and gas industry.

### What you can do

- **Project Management** — List active projects, inspect configurations, and retrieve project-level metadata.
- **Well Search** — Find wells by ID, name, or geographic filters and view production history.
- **Forecast Data** — Retrieve monthly volume forecasts and decline curves for individual wells or full projects.

### How it works

1. Add the ComboCurve integration to your AI toolset.
2. Provide your Service Account credentials (API Key + JWT Bearer Token).
3. Query your energy data via natural language commands.

### Who is this for?

- **Petroleum Engineers** — Pull forecast curves and production volumes without opening the full platform.
- **Financial Analysts** — Extract valuation metrics and well economics for deal evaluation.
- **Operations Teams** — Check well statuses and production trends directly from chat.


## Available Tools (10)
- **get_forecast**: Retrieve details of a specific forecast
- **get_monthly_volumes**: Retrieve monthly forecasted volumes for a project and forecast
- **get_project**: Retrieve details of a specific project
- **get_scenario_details**: Retrieve details of a specific scenario
- **get_well**: Retrieve detailed information about a specific well
- **list_forecasts**: Retrieve a list of forecasts for a specific project
- **list_projects**: Retrieve a list of projects in ComboCurve
- **list_scenarios**: Retrieve a list of scenarios for a specific project
- **list_wells**: Retrieve a list of wells in ComboCurve
- **search_wells_by_name**: Search for wells by name or chosen ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ComboCurve** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active projects in ComboCurve."

**🤖 AI Agent:**
> You have 4 active projects:
1. 'Permian Basin Q1' — 142 wells, last updated today
2. 'Eagle Ford Development' — 87 wells, last updated yesterday
3. 'Delaware Lease Eval' — 34 wells, last updated Jan 18
4. 'Bakken Acquisition' — 56 wells, last updated Jan 15
Would you like forecast data for any of these?

---

**👤 You:**
> "Show monthly volumes for forecast 'fc-yyyy' in project 'proj-xxxx'."

**🤖 AI Agent:**
> Forecast 'fc-yyyy' monthly volumes (oil, bbl):
- Jan 2026: 12,400
- Feb 2026: 11,800
- Mar 2026: 11,200
- Apr 2026: 10,650
Decline rate: ~4.8%/month. Would you like gas and NGL volumes as well?

---

**👤 You:**
> "Get the type curve parameters for the 'Wolfcamp A' formation."

**🤖 AI Agent:**
> Type Curve parameters for 'Wolfcamp A': Initial decline (Di) is 65%, with a b-factor of 1.2, transitioning to a terminal decline (d_term) of 6% at month 36. EUR is estimated at 450 MBOE.


## ❓ FAQ

**Q: How do I get my ComboCurve API key?**
Go to **Admin > API Keys** in the ComboCurve UI and generate a new key. Copy it and paste it below.

**Q: What is the Bearer Token?**
ComboCurve uses a JWT (Bearer Token) generated from a Service Account for authentication. You can generate it using their SDKs or a custom script.

**Q: Can I update well data?**
The current version focuses on reading data. Write operations for wells and forecasts may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/combocurve](https://vinkius.com/mcp/combocurve)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ComboCurve** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `combocurve` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ComboCurve** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "combocurve": {
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
