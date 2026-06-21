# DoiT MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Equip your AI agent to manage cloud costs, track assets across AWS/GCP/Azure, and monitor cost anomalies via the DoiT API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DoiT** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our total cloud cost summary."

**🤖 AI Agent:**
> Your total cloud spending for the current period is $45,200. This includes $22,500 on AWS, $18,700 on GCP, and $4,000 on Azure. Should I list the top service costs for AWS?

---

**👤 You:**
> "Are there any critical cost anomalies right now?"

**🤖 AI Agent:**
> I've detected 2 critical anomalies: a 150% spike in BigQuery costs on GCP and an unexpected increase in S3 data transfer on AWS. Would you like the detailed telemetry for the BigQuery spike?

---

**👤 You:**
> "List all budgets that have exceeded 100% consumption."

**🤖 AI Agent:**
> The 'Dev-Sandbox' and 'Marketing-Analytics' budgets have both exceeded 100% consumption. 'Dev-Sandbox' is currently at 115% of its $2,000 limit. Should I check the associated assets for the Dev-Sandbox account?


## Installation & Usage

To install and use the **DoiT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doit](https://vinkius.com/mcp/doit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
