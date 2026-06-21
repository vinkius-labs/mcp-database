# Coralogix MCP Server

Manage observability, logs, and parsing rules via Coralogix — ingest logs, monitor SLOs, and control Grafana dashboards directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coralogix)

## Overview
**Category:** devops-cicd
**Tools Count:** 17

## Description
Connect your **Coralogix** account to any AI agent to take full control of your observability and log management workflows through natural conversation.

### What you can do

- **Log Ingestion** — Send logs directly to Coralogix with specific severity levels and metadata using `send_logs`.
- **Parsing Rules** — Retrieve, create, or delete log parsing rule groups to restructure your data flow efficiently.
- **SLO Management** — Programmatically create, list, and delete Service Level Objectives (SLOs) to maintain system reliability.
- **TCO Optimization** — Manage Total Cost of Ownership (TCO) policy overrides to optimize log storage and costs.
- **Grafana Integration** — Search and create Grafana dashboards or retrieve the home dashboard configuration.
- **Deployment Tracking** — Mark releases or deployments using version tags to correlate changes with system behavior.

### How it works

1. Subscribe to this server
2. Enter your Coralogix API Key and Domain
3. Start managing your observability stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the creation of parsing rules and monitor SLOs without leaving the terminal or chat.
- **SREs** — quickly check TCO overrides and deployment tags during incident response.
- **Developers** — send application logs and verify dashboard configurations directly from the code editor.


## Available Tools
- **get_rules**: Get all parsing rules
- **get_tco_overrides**: Get all TCO policy overrides
- **list_custom_enrichments**: List custom enrichments
- **list_slos**: List all SLOs
- **search_grafana_dashboards**: Search hosted Grafana dashboards
- **create_rule_group**: Create a parsing rule group
- **create_slo**: Create a Service Level Objective (SLO)
- **create_tco_override**: Create a TCO policy override
- **send_logs**: Provide an array of log objects.

Send logs to Coralogix
- **create_version_tag**: Create a version tag
- **delete_custom_enrichment**: Delete a custom enrichment
- **delete_rule_group**: Delete a parsing rule group
- **delete_slo**: Delete an SLO
- **delete_tco_override**: Delete a TCO policy override
- **get_grafana_home**: Get hosted Grafana home dashboard
- **get_rule_group**: Get a specific parsing rule group
- **create_grafana_dashboard**: Create or update a hosted Grafana dashboard


## Installation & Usage

To install and use the **Coralogix** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coralogix](https://vinkius.com/mcp/coralogix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
