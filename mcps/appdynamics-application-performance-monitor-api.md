# AppDynamics (Application Performance Monitor API) MCP Server

Monitor application performance, business transactions, and infrastructure health rules directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/appdynamics-application-performance-monitor-api)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 13

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


## Installation & Usage

To install and use the **AppDynamics (Application Performance Monitor API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appdynamics-application-performance-monitor-api](https://vinkius.com/mcp/appdynamics-application-performance-monitor-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
