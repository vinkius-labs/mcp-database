# DoiT MCP Server

Equip your AI agent to manage cloud costs, track assets across AWS/GCP/Azure, and monitor cost anomalies via the DoiT API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/doit)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Integrate **DoiT**, the leading cloud cost management and optimization platform, directly into your AI workflow. Manage your multi-cloud assets across AWS, Google Cloud, and Microsoft Azure, monitor real-time cost anomalies and budgets, and track your cloud spending using natural language.

### What you can do

- **Cloud Oversight** — List and retrieve detailed configuration and cost data for all your cloud assets and connected accounts.
- **Anomaly Intelligence** — Monitor real-time cost anomalies and unexpected spending spikes across your cloud infrastructure.
- **Budget Monitoring** — Track cloud spending budgets, threshold limits, and current consumption percentages.
- **Cost Auditing** — Retrieve high-level summaries of total cloud expenditure and identify high-severity cost spikes instantly.

### How it works

1. Connect the DoiT integration to your AI assistant.
2. Authorize using your DoiT API Key (found in your organization settings).
3. Orchestrate your cloud cost management and resource optimization through intuitive conversation.

### Who is this for?

- **FinOps Teams** — Quickly check budget status and total cloud spending on the go.
- **Cloud Architects** — Audit multi-cloud asset configurations and platform associations via chat.
- **Operations Leads** — Monitor cost anomalies and critical spending alerts across the organization instantly.


## Available Tools
- **get_doit_account_metadata**: Retrieve metadata for the current DoiT organization
- **get_asset_details**: Get detailed configuration and cost data for a specific cloud asset
- **get_billing_cost_summary**: Retrieve a high-level summary of total cloud spending across all platforms
- **list_cost_anomalies**: List all detected cloud cost anomalies and unexpected spending spikes
- **list_cloud_assets**: List all cloud assets (AWS, GCP, Azure) managed by DoiT
- **list_cost_budgets**: List all cloud spending budgets configured in DoiT
- **list_connected_cloud_accounts**: List all connected AWS, GCP, or Azure accounts
- **list_critical_cost_spikes**: Identify high-severity cost anomalies that require immediate attention
- **list_exceeded_cost_budgets**: Identify budgets that have exceeded their configured spending limits
- **search_cloud_assets**: Search for cloud assets using a name keyword


## Installation & Usage

To install and use the **DoiT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doit](https://vinkius.com/mcp/doit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
