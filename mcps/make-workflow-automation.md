# Make (Workflow Automation) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/make-workflow-automation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/make-workflow-automation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/make-workflow-automation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage workflow automation via Make — audit scenarios, track execution logs, and monitor data stores.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Make (Workflow Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Make account"

**🤖 AI Agent:**
> I've retrieved your Make organizations: 'Personal Workspace' (ID: 12345) and 'Corporate Ops' (ID: 67890). Which one would you like to list scenarios for?

---

**👤 You:**
> "Show me the execution logs for scenario ID 'scen-98765'"

**🤖 AI Agent:**
> Retrieving logs for 'Shopify-to-Slack-Sync'… The last run was 5 minutes ago and completed successfully. However, 2 hours ago there was a '401 Unauthorized' error on the Slack module. Would you like to see the detailed error payload?

---

**👤 You:**
> "List all active connections in organization '12345'"

**🤖 AI Agent:**
> I've identified 5 active connections in organization 12345: Google Sheets (Verified), Slack (Verified), Airtable (Expired), HubSpot (Verified), and Mailchimp (Verified). You might want to re-authenticate your Airtable connection.


## Installation & Usage

To install and use the **Make (Workflow Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/make-workflow-automation](https://vinkius.com/mcp/make-workflow-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
