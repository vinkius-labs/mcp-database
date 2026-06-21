# ComboCurve MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/combocurve)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/combocurve-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/combocurve-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **ComboCurve** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/combocurve](https://vinkius.com/mcp/combocurve)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
