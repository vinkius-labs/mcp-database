# New Relic MCP Server

Monitor and query your entire stack via New Relic NerdGraph — track entities, NRQL, and alerts directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/new-relic)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **New Relic** account to your AI agent and gain full visibility into your applications and infrastructure through natural conversation using the powerful NerdGraph GraphQL API.

### What you can do

- **Entity Discovery** — List and search for monitored entities such as APM applications, hosts, containers, and browser apps.
- **Custom Querying** — Execute raw NRQL (New Relic Query Language) strings to retrieve specific datasets and custom metrics.
- **Golden Metrics** — Fetch real-time APM summaries including error rates, Apdex scores, and average response times.
- **Incident Monitoring** — Track active AI-detected issues and open alerts across your accounts.
- **Dashboard Oversight** — List and retrieve configuration details for your custom observability dashboards.
- **Account Management** — Access current user metadata and list all accessible New Relic accounts.
- **SLO Tracking** — Monitor defined Service Level Indicators (SLOs) and performance levels.

### How it works

1. Subscribe to this server
2. Enter your New Relic User API Key
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **SRE & DevOps Engineers** — quickly check for active incidents or run NRQL queries without opening the browser.
- **Developers** — monitor the health and golden metrics of your applications during deployment or testing.
- **Product Managers** — track SLOs and high-level performance indicators through natural language.


## Available Tools
- **get_apm_summary**: Get APM golden metrics
- **get_dashboard**: Get dashboard configuration
- **get_entity_details**: Get specific entity metadata
- **get_me**: Get current user and account info
- **list_accounts**: List accessible New Relic accounts
- **list_alerts**: List active issues and alerts
- **list_dashboards**: List New Relic dashboards
- **list_entities**: List monitored entities
- **list_service_levels**: List Service Level Indicators (SLOs)
- **run_nrql**: Execute a NRQL query


## Installation & Usage

To install and use the **New Relic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/new-relic](https://vinkius.com/mcp/new-relic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
