# LinearB MCP Server

Export software delivery metrics, manage deployments, and report incidents via the LinearB API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/linearb)

## Overview
**Category:** ship-it
**Tools Count:** 7

## Description
Connect your **LinearB** account to any AI agent to automate your engineering intelligence and DORA metrics reporting. This MCP server enables your agent to query cycle time, track deployments, and report incidents directly from natural language interfaces.

### What you can do

- **Metric Ingestion** — Query complex engineering metrics including cycle time, coding time, and pickup time across teams
- **Deployment Management** — Inform LinearB of new software releases by reporting Git refs (SHAs or tags) programmatically
- **Incident Tracking** — Report and list engineering incidents to maintain accurate Change Failure Rate and MTTR metrics
- **Metadata Oversight** — List teams and connected repositories to map technical IDs to organizational structures
- **DORA Analytics** — Retrieve aggregated performance data to identify bottlenecks in your delivery pipeline

### How it works

1. Subscribe to this server
2. Enter your LinearB Public API Key
3. Start managing your engineering metrics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Managers** — Monitor team cycle times and delivery health via simple natural language commands
- **DevOps Engineers** — Automate the reporting of deployments and incidents directly from CI/CD pipelines or IDEs
- **CTOs** — Quickly audit organizational performance and DORA metrics without opening the dashboard


## Available Tools
- **record_new_deployment**: Requires repo_id and ref.

Report a new deployment to LinearB
- **record_new_incident**: Requires provider_id and started_at.

Report a new incident
- **list_software_deployments**: List recent deployments
- **list_software_incidents**: List engineering incidents
- **query_software_metrics**: Requires a JSON body with requested_metrics and time_ranges.

Query software engineering metrics (v2)
- **list_connected_repos**: List all connected repositories
- **list_engineering_teams**: List all teams defined in LinearB


## Installation & Usage

To install and use the **LinearB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linearb](https://vinkius.com/mcp/linearb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
