# Dynatrace (APM and Observability) MCP Server

Monitor and manage your Dynatrace environment — query metrics, track problems, manage entities, and automate observability workflows directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dynatrace-apm-and-observability)

## Overview
**Category:** devops-cicd
**Tools Count:** 37

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


## Installation & Usage

To install and use the **Dynatrace (APM and Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynatrace-apm-and-observability](https://vinkius.com/mcp/dynatrace-apm-and-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
