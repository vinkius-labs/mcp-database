# Make (Workflow Automation) MCP Server

Manage workflow automation via Make — audit scenarios, track execution logs, and monitor data stores.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/make-workflow-automation)

## Overview
**Category:** growth-engine
**Tools Count:** 7

## Description
Connect your **Make** account to any AI agent and take full control of your visual workflow automation and scenario management through natural conversation.

### What you can do

- **Scenario Orchestration** — List all managed scenarios and retrieve detailed flow design structures, including module mappings and trigger settings directly from your agent
- **Execution Diagnostics** — Extract historical scenario logs to identify errors, track data processing volumes, and debug automation failures in real-time
- **Infrastructure Audit** — Enumerate active organizations, teams, and connections to understand your automation footprint and verify authentication hooks securely
- **Data Store Visibility** — List and inspect internal Make Data stores (key-value tables) to monitor persistent data used across your automated workflows
- **Environment Mapping** — Retrieve precise organization and team IDs required for complex downstream API operations and organizational auditing
- **Metadata Inspection** — Deep-dive into specific scenario configurations to understand the logic and logic loops powering your business processes

### How it works

1. Subscribe to this server
2. Enter your Make API Token and Zone (e.g., eu1, us1)
3. Start managing your automation infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Automation Engineers** — verify scenario designs and audit connection statuses through natural conversation without manual dashboard navigation
- **Ops Managers** — monitor execution logs and scenario health across multiple teams to ensure business process reliability
- **Developers** — inspect data store contents and retrieve scenario metadata directly from your workspace for rapid debugging


## Available Tools
- **list_scenarios**: Check the list of organizations if org_id is unknown.

List Make scenarios
- **get_scenario**: Get Make scenario details
- **list_organizations**: List Make organizations for the current authenticated user
- **list_connections**: List Make connections linked to an organization
- **list_teams**: Needs org_id.

List Make teams inside an organization
- **list_scenario_logs**: Helps debug automation errors.

Get execution logs of a Make scenario
- **list_data_stores**: List Make data stores


## Installation & Usage

To install and use the **Make (Workflow Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/make-workflow-automation](https://vinkius.com/mcp/make-workflow-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
