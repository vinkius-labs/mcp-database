# Raygun MCP Server

Monitor application health, track deployments, and manage crash reports and RUM sessions directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/raygun)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Connect your **Raygun** account to any AI agent to gain deep visibility into your application's performance and stability through natural language.

### What you can do

- **Application Management** — List all accessible applications and environments within your Raygun account.
- **Deployment Tracking** — Monitor and list deployments for specific applications to correlate releases with performance changes.
- **Crash Reporting** — Manually send crash reports and error payloads to the Raygun API for centralized tracking.
- **Real User Monitoring (RUM)** — Authenticate and search through user sessions to understand real-world performance and user journeys.
- **Session Inspection** — Retrieve detailed metadata for specific RUM sessions to debug user-specific issues.

### How it works

1. Subscribe to this server
2. Enter your Raygun Personal Access Token (PAT) or API Key
3. Start monitoring your stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — Quickly check deployment history and application health without leaving the terminal or chat.
- **Software Engineers** — Send manual crash reports during testing or inspect RUM sessions to reproduce bugs.
- **Product Owners** — Query user session data to understand how new features are performing in the wild.


## Available Tools
- **create_legacy_deployment**: Create a deployment using the legacy API
- **list_applications**: List accessible Raygun applications
- **list_deployments**: List deployments for a specific application
- **rum_authenticate**: Authenticate with the legacy RUM API
- **rum_get_session**: Get RUM session details
- **rum_search_sessions**: Search RUM sessions
- **send_crash_report**: Send a manual crash report to Raygun


## Installation & Usage

To install and use the **Raygun** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/raygun](https://vinkius.com/mcp/raygun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
