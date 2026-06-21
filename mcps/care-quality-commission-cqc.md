# Care Quality Commission (CQC) MCP Server

Access UK health and social care regulator data via CQC — search providers, check ratings, and retrieve inspection reports directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/care-quality-commission-cqc)

## Overview
**Category:** government-public-data
**Tools Count:** 8

## Description
Connect your AI agent to the **Care Quality Commission (CQC)** Syndication API and orchestrate your health and social care research in England through natural conversation. Retrieve real-time data on hospitals, care homes, and clinics.

### What you can do

- **Provider Discovery** — Search for registered health and social care providers by name across England
- **Location Intelligence** — Find care locations by postcode or proximity to identify local services
- **Quality Oversight** — Retrieve the latest CQC ratings (Outstanding, Good, Requires Improvement, Inadequate) for any registered service
- **Inspection Reports** — Get detailed summaries and links to the latest inspection findings and compliance reports
- **Change Monitoring** — Track updates and changes in registration or ratings within specific timeframes
- **Structural Mapping** — Map providers to their specific registered locations to understand organizational structures

### How it works

1. Subscribe to this server
2. Enter your CQC Ocp-Apim-Subscription-Key (obtained from the CQC Developer Portal)
3. Start querying UK health care data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Analysts** — gather data on care provider performance and registration status for market research
- **Social Care Planners** — identify and evaluate local care services based on official quality ratings
- **Compliance Officers** — monitor changes in ratings or registration status for a portfolio of care locations
- **Developers** — integrate official health regulation data into healthcare management applications


## Available Tools
- **get_changes**: Identify organizations updated within a specific timeframe
- **get_location**: Get detailed information for a specific location, including ratings
- **get_provider_locations**: Get all locations associated with a specific provider
- **get_provider**: Get detailed information for a specific provider
- **list_locations**: List all registered locations (hospitals, care homes, clinics)
- **list_providers**: List registered health and social care providers
- **search_locations_by_postcode**: Search for locations by postcode
- **search_providers**: Search for providers by name


## Installation & Usage

To install and use the **Care Quality Commission (CQC)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/care-quality-commission-cqc](https://vinkius.com/mcp/care-quality-commission-cqc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
