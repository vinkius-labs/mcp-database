# HCSS MCP Server

Automate heavy construction management via HCSS — manage jobs, timecards, estimates, and equipment telematics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hcss)

## Overview
**Category:** erp-operations
**Tools Count:** 11

## Description
Connect your **HCSS** platform to any AI agent and take full control of your heavy construction workflows, from estimating to field data and equipment tracking, through natural conversation.

### What you can do

- **Field Data Management** — List construction jobs and retrieve timecard data from HeavyJob to monitor site progress.
- **Estimating Insights** — Access bidding estimates and bid items from HeavyBid to stay aligned with project budgets.
- **Equipment Telematics** — Monitor your fleet with real-time GPS locations and latest meter readings (odometer/hours).
- **Resource Coordination** — List employees and business units defined across the HCSS ecosystem.
- **Pre-Construction Tracking** — Browse active pre-con projects and project lifecycles.
- **Operational Efficiency** — Use AI to identify equipment utilization trends or job cost variances in seconds.

### How it works

1. Subscribe to this server
2. Enter your HCSS Client ID, Client Secret, and API Key (Subscription Key)
3. Start managing your construction projects from Claude, Cursor, or any MCP-compatible client

No more manual exporting of field reports or logging into multiple portals. Your AI assistant acts as a dedicated Project Engineer or Fleet Manager.

### Who is this for?

- **Project Managers** — instantly retrieve job costs and timecard statuses straight from the field.
- **Fleet Managers** — check equipment locations and maintenance needs without digging through telematics screens.
- **Estimators** — verify bid item details and estimate progress during high-pressure bidding cycles.


## Available Tools
- **get_bid_items**: List bid items for a specific estimate
- **get_equipment_location**: Get current GPS coordinates for a specific piece of equipment
- **get_equipment_meters**: Get latest meter readings (odometer/hours) for equipment
- **list_business_units**: List all business units in HCSS
- **list_cost_codes**: List cost codes defined in the system
- **list_employees**: List all employees synced in HCSS
- **list_equipment**: List all tracked equipment/fleet from Telematics
- **list_estimates**: List bidding estimates from HeavyBid
- **list_jobs**: List all construction jobs/projects
- **list_precon_projects**: List active pre-construction projects
- **list_timecards**: List timecards from HeavyJob


## Installation & Usage

To install and use the **HCSS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hcss](https://vinkius.com/mcp/hcss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
