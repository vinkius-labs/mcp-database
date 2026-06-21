# SigNoz (Datadog Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signoz-datadog-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/signoz-datadog-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/signoz-datadog-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor infrastructure and manage alert rules via SigNoz — list, create, and update observability alerts directly from your AI agent.

## Description
Connect your **SigNoz** instance to any AI agent to streamline your observability and monitoring workflows. SigNoz provides a powerful open-source alternative to Datadog, and this server allows you to manage your alerting infrastructure through natural conversation.

### What you can do

- **Alert Rule Management** — List all configured alert rules, create new ones, or update existing thresholds and conditions using JSON payloads.
- **Rule Maintenance** — Quickly delete stale or redundant alert rules to keep your monitoring environment clean.
- **Account Validation** — Verify your current service account details and API key permissions instantly to ensure connectivity.
- **Observability Audit** — Fetch all alert configurations to audit your monitoring stack without leaving your code editor.

### How it works

1. Subscribe to this server
2. Enter your SigNoz Instance URL and API Key
3. Start managing your monitoring stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the creation of alert rules during deployment or scaling cycles.
- **SREs** — quickly audit existing alert thresholds and conditions without navigating complex web UIs.
- **Platform Teams** — manage observability configurations across multiple environments via simple chat commands.


## Available Tools
- **create_rule**: g., alert, alert_type, condition, thresholds).

Create a new alert rule
- **delete_rule**: Delete an alert rule
- **get_service_account_me**: Get current service account details
- **list_rules**: Retrieve all configured alert rules
- **update_rule**: Update an existing alert rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SigNoz (Datadog Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all alert rules in my SigNoz instance."

**🤖 AI Agent:**
> I've retrieved 8 alert rules. Some active rules include 'High CPU Usage' (ID: 1), 'Database Latency' (ID: 2), and 'Service 5xx Errors' (ID: 3). Would you like to see the details for any specific rule?

---

**👤 You:**
> "Show me the details of my current service account."

**🤖 AI Agent:**
> Your API key is valid. You are connected as 'Monitoring-Admin' with the following permissions: [Alerts: Read/Write, Dashboards: Read]. Your account ID is 'sa-99283'.

---

**👤 You:**
> "Delete the alert rule with ID 'alert-123'."

**🤖 AI Agent:**
> The alert rule 'alert-123' has been successfully deleted from your SigNoz instance.


## Installation & Usage

To install and use the **SigNoz (Datadog Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signoz-datadog-alternative](https://vinkius.com/mcp/signoz-datadog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
