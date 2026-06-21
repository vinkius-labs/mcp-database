# Insightful MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/insightful)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/insightful-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/insightful-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee productivity, time tracking, and activity via Insightful API.

## Description
Empower your AI agents to analyze and manage workforce productivity with Insightful (formerly Workpuls). This MCP server allows you to list employees and teams, track project progress, monitor real-time activity, and retrieve productivity and attendance reports directly through the Insightful API. Ideal for automating team management and performance monitoring.


## Available Tools
- **get_attendance**: Retrieves aggregated attendance and time tracking reports
- **get_employee**: Retrieves details for a specific employee
- **get_productivity**: Retrieves aggregated productivity reports
- **list_activity**: Lists recent employee activity logs
- **list_employees**: Lists all employees in the organization
- **list_locations**: Lists all registered organization locations
- **list_projects**: Lists all active and past projects
- **list_tasks**: Lists all tasks across projects
- **list_teams**: Lists all organization teams
- **list_webhooks**: Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insightful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the 'Engineering' team."

**🤖 AI Agent:**
> I'll fetch the employee list and filter for the engineering team from Insightful.

---

**👤 You:**
> "Show me the productivity report for last week."

**🤖 AI Agent:**
> I'll retrieve the aggregated productivity metrics for your organization.

---

**👤 You:**
> "Check recent activity logs for project ID '789'."

**🤖 AI Agent:**
> I'll look up the activity logs associated with that specific project.


## Installation & Usage

To install and use the **Insightful** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/insightful](https://vinkius.com/mcp/insightful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
