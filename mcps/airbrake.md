# Airbrake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airbrake)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airbrake-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airbrake-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Catch application errors in real time, track performance bottlenecks, and keep your codebase healthy with proactive monitoring.

## Description
Connect your **Airbrake** account to any AI agent and manage your entire error monitoring workflow through natural conversation.

### What you can do

- **Project Management** — List all monitored projects and fetch detailed project configuration
- **Error Group Analysis** — List error groups by project with occurrence counts, severity, and last-seen timestamps
- **Deep Error Inspection** — Inspect individual error groups with full stack traces, affected users, and frequency data
- **Error Notices** — List individual error occurrences within a group and report custom errors for tracking
- **Deployment Tracking** — List all tracked Installments and record new releases with version and environment info
- **Environment Overview** — View all configured environments (production, staging, development) per project
- **Health Check** — Verify API connectivity and account status

### How it works

1. Subscribe to this server
2. Enter your **API Key** from your Airbrake account settings
3. Start monitoring errors from Claude, Cursor, or any MCP client

### Who is this for?

- **Engineering Teams** — investigate error spikes and review stack traces without leaving the code editor
- **DevOps** — track deployments and correlate releases with error rates
- **QA Teams** — monitor error groups across environments and report custom test failures


## Available Tools
- **check_airbrake_status**: Verify API connectivity
- **get_error_group**: Get error group details
- **get_project**: Get project details
- **list_deploys**: List deployments
- **list_environments**: List environments
- **list_error_groups**: List error groups
- **list_notices**: List error notices
- **list_projects**: List all projects
- **report_notice**: Report an error notice
- **track_deploy**: Track a deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airbrake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Airbrake projects."

**🤖 AI Agent:**
> You have 4 projects: 'API Gateway' (ID: 120394, 23 active error groups), 'Frontend App' (ID: 120395, 8 groups), 'Worker Service' (ID: 120396, 15 groups), and 'Mobile SDK' (ID: 120397, 3 groups). Which project would you like to investigate?

---

**👤 You:**
> "Show me the error groups for project 120394."

**🤖 AI Agent:**
> Project 'API Gateway' has 23 error groups. Top 3 by occurrence: 'TimeoutError' (1,847 occurrences, last seen 2 min ago), 'ConnectionRefused' (523 occurrences, last seen 15 min ago), 'ValidationError' (189 occurrences, last seen 1 hour ago). Would you like to inspect the stack trace of the TimeoutError?

---

**👤 You:**
> "Record a Installment for project 120394: version 3.2.1, production."

**🤖 AI Agent:**
> Installment recorded! Version 3.2.1 has been tracked in production for project 'API Gateway'. Airbrake will now correlate new errors with this release. Would you like to check the error rate after this Install?


## Installation & Usage

To install and use the **Airbrake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airbrake](https://vinkius.com/mcp/airbrake)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
