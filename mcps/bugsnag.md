# BugSnag MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugsnag)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bugsnag-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bugsnag-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Monitor application errors via BugSnag — track stability, inspect error groups, and retrieve event details directly from any AI agent.

## Description
Connect your **BugSnag** account to any AI agent and orchestrate your error monitoring, stability tracking, and incident response workflows through natural conversation.

### What you can do

- **Organization Oversight** — List all your organizations and projects to maintain visibility across your entire tech stack.
- **Error Management** — List and inspect error groups for specific projects, including error classes, severity, and frequency.
- **Event Deep Dives** — Retrieve individual error events and occurrence details to debug issues faster.
- **Team Coordination** — Access your directory of collaborators and release stages to ensure everyone is aligned.
- **Stability Insights** — Retrieve error trends and statistics to monitor the health of your applications over time.
- **Incident Response** — Get detailed metadata for specific error or event IDs straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BugSnag Personal Auth Token
3. Start monitoring your application stability from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — quickly check error details or event counts without manual dashboard searches.
- **SREs & DevOps** — monitor stability trends and release stage health straight from their workflow tools.
- **Product Managers** — retrieve high-level error statistics using natural language.


## Available Tools
- **get_error**: Get details of a specific error group
- **get_event**: Get details of a specific error event
- **get_project**: Get details of a specific project
- **get_project_stats**: Get error trends and statistics for a project
- **list_collaborators**: List collaborators in an organization
- **list_errors**: List error groups for a project
- **list_events**: List individual error events for a project
- **list_organizations**: List all organizations you have access to
- **list_projects**: List all projects in an organization
- **list_release_stages**: List release stages configured for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BugSnag** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my projects in BugSnag for organization org_123."

**🤖 AI Agent:**
> I've retrieved your projects for 'Vinkius Org'. You have 3 projects: 'iOS App' (ID: proj_1), 'Android App' (ID: proj_2), and 'Web Dashboard' (ID: proj_3).

---

**👤 You:**
> "Show the last 5 errors for the 'Web Dashboard' project."

**🤖 AI Agent:**
> Retrieving errors... Your 5 most recent error groups include 'TypeError: undefined is not a function' (Severity: Error) and 'NetworkError: Failed to fetch' (Severity: Warning).

---

**👤 You:**
> "Get details for error group err_99283."

**🤖 AI Agent:**
> Error err_99283 is a 'ReferenceError' that has occurred 150 times in the last 24 hours. It is currently affecting 45 users in production.


## Installation & Usage

To install and use the **BugSnag** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugsnag](https://vinkius.com/mcp/bugsnag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
