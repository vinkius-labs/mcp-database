# AppDynamics (Application Performance Monitor API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appdynamics-application-performance-monitor-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor application performance, business transactions, and infrastructure health rules directly from your AI agent.

## Description
Connect your **AppDynamics** Controller to any AI agent to gain deep visibility into your software ecosystem through natural language. This MCP server provides a comprehensive interface to the AppDynamics Application Performance Monitor API.

### What you can do

- **Application Discovery** — List all applications, tiers, and nodes monitored by your Controller to map out your infrastructure.
- **Performance Metrics** — Retrieve real-time metric data (like Average Response Time or Errors per Minute) using specific metric paths.
- **Transaction Monitoring** — List business transactions and access detailed snapshots to identify bottlenecks.
- **Health & Compliance** — Export health rules and monitor violations to ensure your system stays within operational thresholds.
- **User Management** — List and create users within the Controller to manage access and collaboration.

### How it works

1. Subscribe to this server
2. Provide your AppDynamics Controller URL, Username, and Password
3. Start querying your APM data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SREs & DevOps Engineers** — quickly check system health and metric rollups without navigating the Controller UI.
- **Developers** — inspect transaction snapshots and node performance directly from the IDE during debugging.
- **IT Operations** — automate health rule reporting and user auditing via conversational commands.


## Available Tools
- **list_applications**: List all applications monitored by the Controller
- **list_business_transactions**: List business transactions for an application
- **create_event**: Create a custom event
- **create_user**: Create a new Controller user
- **list_custom_match_rules**: Manage custom match rules
- **export_health_rules**: Export health rules for an application
- **list_health_rule_violations**: List health rule violations
- **import_health_rules**: Import health rules for an application
- **list_users**: List all Controller users
- **get_metric_data**: Retrieve metric data for an application
- **list_nodes**: List nodes within an application
- **list_snapshots**: Retrieve transaction snapshots
- **list_tiers**: List tiers within an application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppDynamics (Application Performance Monitor API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications monitored by our AppDynamics Controller."

**🤖 AI Agent:**
> I've retrieved the applications. You have 3 active applications: 'E-Commerce-Prod' (ID: 45), 'Payment-Gateway' (ID: 12), and 'Inventory-Service' (ID: 89).

---

**👤 You:**
> "Show me the average response time for application 45 for the last 15 minutes."

**🤖 AI Agent:**
> Fetching metric data... The Average Response Time for 'E-Commerce-Prod' over the last 15 minutes is 245ms, with a peak of 410ms during the last 5-minute window.

---

**👤 You:**
> "Are there any health rule violations for app 12?"

**🤖 AI Agent:**
> Checking violations... I found one 'Warning' violation for 'Payment-Gateway': 'CPU Usage is high on Tier: Web-FrontEnd'. It started 10 minutes ago.


## ❓ FAQ

**Q: How can I check the average response time for a specific application?**
You can use the `get_metric_data` tool. Provide the `app_id` and the `metric_path` (e.g., 'Overall Application Performance|Average Response Time (ms)') to retrieve precise performance data.

**Q: Can I see which server instances (nodes) are currently active in an application?**
Yes! Use the `list_nodes` tool with the target `app_id`. It will return all individual server instances associated with that application.

**Q: Is it possible to audit health rules through the AI?**
Absolutely. Use `export_health_rules` to retrieve the current configuration for an application, or `list_health_rule_violations` to see active issues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appdynamics-application-performance-monitor-api](https://vinkius.com/mcp/appdynamics-application-performance-monitor-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppDynamics (Application Performance Monitor API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `appdynamics-application-performance-monitor-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppDynamics (Application Performance Monitor API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appdynamics-application-performance-monitor-api": {
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
