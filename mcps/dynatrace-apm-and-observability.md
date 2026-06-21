# Dynatrace (APM and Observability) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dynatrace-apm-and-observability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Monitor and manage your Dynatrace environment — query metrics, track problems, manage entities, and automate observability workflows directly from your AI agent.

## Description
Connect your **Dynatrace** environment to any AI agent to gain deep visibility into your software ecosystem. This server provides comprehensive access to the Dynatrace Environment API (v2), allowing for real-time monitoring, problem analysis, and infrastructure management through natural language.

### What you can do

- **Metrics & Events** — Query performance data points using metric selectors and ingest custom events or metrics directly into your environment.
- **Problem Management** — List active or closed problems, retrieve deep technical details for specific issues, and close resolved problems programmatically.
- **Entity Discovery** — List and filter monitored entities like hosts, services, and applications to understand your infrastructure topology.
- **Synthetic Monitoring** — Manage synthetic monitors and locations, trigger execution batches, and track performance from different geographic points.
- **Dashboarding & Settings** — Create, update, or delete dashboards and manage environment settings schemas and objects.
- **Account Administration** — Manage users, groups, policies, and permissions across your Dynatrace account.

### How it works

1. Subscribe to this server
2. Enter your Dynatrace Environment URL and API Token
3. Start querying your observability data from Claude, Cursor, or any MCP client

### Who is this for?

- **SRE & DevOps Engineers** — Automate incident response by fetching problem details and metric data points directly in the terminal or chat.
- **Platform Teams** — Manage infrastructure entities and synthetic monitors without switching between multiple browser tabs.
- **IT Managers** — Generate quick reports on environment health and user access policies through simple conversation.


## Available Tools
- **create_synthetic_location**: Create a synthetic location
- **create_synthetic_monitor**: Create a synthetic monitor
- **delete_dashboard**: Delete a dashboard
- **delete_synthetic_location**: Delete a synthetic location
- **delete_synthetic_monitor**: Delete a synthetic monitor
- **get_anomaly_detection_apps**: Get anomaly detection configuration for applications
- **get_anomaly_detection_hosts**: Get anomaly detection configuration for hosts
- **get_anomaly_detection_services**: Get anomaly detection configuration for services
- **get_calculated_metrics_service**: Get calculated service metrics configuration
- **get_problem**: Get details of a specific problem
- **ingest_events**: Ingest custom events into Dynatrace
- **ingest_metrics**: Push custom data points using the line protocol
- **list_account_groups**: List user groups in an account
- **list_account_policies**: List access policies in an account
- **list_account_users**: List all users in an account
- **list_dashboards**: List all dashboards
- **list_entities**: List monitored entities
- **list_entity_types**: List all available entity types
- **list_events**: List events within a timeframe
- **list_metrics**: List available metrics
- **list_problems**: List open and closed problems
- **list_settings_objects**: List configuration objects
- **list_settings_schemas**: List all configuration schemas
- **list_synthetic_executions**: View results of monitor runs
- **list_synthetic_locations**: List synthetic locations
- **list_synthetic_monitors**: List synthetic monitors
- **query_metrics**: Query data points for specific metrics
- **trigger_synthetic_batch**: Trigger immediate execution of synthetic monitors
- **update_account_group_permissions**: Manage group permissions
- **update_dashboard**: Update an existing dashboard
- **update_synthetic_location**: Update a synthetic location
- **update_synthetic_monitor**: Update a synthetic monitor
- **close_problem**: Manually close a problem
- **create_account_policy**: Create a custom access policy
- **create_account_user**: Create a new user in an account
- **create_custom_entity**: Create or update custom devices
- **create_dashboard**: Create a new dashboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dynatrace (APM and Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active problems in my Dynatrace environment."

**🤖 AI Agent:**
> I've found 3 active problems. The most critical is 'High CPU saturation' on host 'Production-Web-01'. Would you like me to get the full details for this problem?

---

**👤 You:**
> "Query the average CPU usage metric for the last hour."

**🤖 AI Agent:**
> Querying `builtin:host.cpu.usage:avg`... The average CPU usage across your monitored hosts is currently 42%, with a peak of 88% on your database cluster.

---

**👤 You:**
> "Show me all monitored entities of type HOST."

**🤖 AI Agent:**
> I've retrieved the list of monitored hosts. You have 12 active hosts, including 'App-Server-01', 'DB-Primary', and 10 worker nodes. All are currently reporting as healthy.


## ❓ FAQ

**Q: How can I check for active problems in my environment?**
You can use the `list_problems` tool. It retrieves all open and closed problems detected by Dynatrace, providing you with an immediate overview of your system's health.

**Q: Is it possible to query specific performance metrics like CPU usage?**
Yes! Use the `query_metrics` tool with a metric selector (e.g., `builtin:host.cpu.usage:avg`). The agent will fetch the relevant data points for analysis.

**Q: Can I manage my synthetic monitoring tests through this server?**
Absolutely. You can use `list_synthetic_monitors` to see your current tests and `trigger_synthetic_batch` to manually start execution sequences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynatrace-apm-and-observability](https://vinkius.com/mcp/dynatrace-apm-and-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dynatrace (APM and Observability)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dynatrace-apm-and-observability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dynatrace (APM and Observability)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dynatrace-apm-and-observability": {
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
