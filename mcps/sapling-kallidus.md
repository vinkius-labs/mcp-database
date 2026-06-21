# Sapling (Kallidus) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sapling-kallidus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sapling-kallidus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sapling-kallidus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee onboarding, data, and tasks via Sapling API.

## Description
Empower your AI agents with Sapling's (by Kallidus) HR and onboarding platform. This MCP server allows you to list and retrieve employee profiles, track onboarding and offboarding tasks, manage departments and teams, and view office locations directly through the Sapling API. Ideal for automating HR workflows and personnel management.


## Available Tools
- **get_account**: Use to verify connection status and account settings.

Retrieves details about your Sapling account
- **get_employee**: Returns employment history, compensation details (if available), and custom attributes. Essential for deep intelligence on an individual team member.

Retrieves details for a specific employee
- **list_departments**: g., Engineering, HR, Sales) defined in Sapling. Useful for mapping the company structure.

Lists all departments
- **list_employees**: Returns names, emails, and internal IDs. Use this as the main starting point for HR auditing or personnel lookups.

Lists all employees in Sapling
- **list_groups**: Lists all custom employee groups
- **list_job_titles**: Useful for standardized role auditing.

Lists all configured job titles
- **list_locations**: Useful for auditing site-based employee distribution.

Lists all office locations
- **list_offboarding_tasks**: Essential for ensuring secure and compliant offboarding workflows.

Lists all offboarding tasks
- **list_onboarding_tasks**: Essential for monitoring the progress of new hire integrations.

Lists all onboarding tasks
- **list_teams**: Useful for understanding internal team organization beyond departments.

Lists all internal teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sapling (Kallidus)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in Sapling."

**🤖 AI Agent:**
> I'll fetch the complete list of employees from your Sapling HR account.

---

**👤 You:**
> "Show me the onboarding tasks for new hires."

**🤖 AI Agent:**
> I'll retrieve the list of active onboarding tasks from Sapling.

---

**👤 You:**
> "Get details for employee ID '123'."

**🤖 AI Agent:**
> I'll retrieve the full HR profile and history for that specific employee.


## Installation & Usage

To install and use the **Sapling (Kallidus)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sapling-kallidus](https://vinkius.com/mcp/sapling-kallidus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
