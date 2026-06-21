# Jibble MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jibble)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jibble-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jibble-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Track time, attendance, and projects via Jibble API.

## Description
Empower your AI agents with Jibble's time tracking and attendance platform. This MCP server allows you to list time entries, retrieve person details, track activities and projects, and view organization information directly through the Jibble API. Ideal for automating workforce management and productivity analysis.


## Available Tools
- **get_organization**: Use to verify account-wide configuration.

Retrieves organization details
- **get_person**: Essential for detailed HR analysis of an individual team member.

Retrieves details for a specific person
- **get_time_entry**: Returns location data, activity notes, and associated device info. Use for auditing or correcting a specific employee time log.

Retrieves details for a specific time entry
- **list_activities**: g., "Meeting", "Development", "Break") that employees can select when clocking in. Useful for identifying high-level task categories.

Lists all configured activities
- **list_clients**: Useful for professional services tracking and billable hours auditing.

Lists all configured clients
- **list_groups**: g., "Sales Team", "Remote Workers") used to organize the workforce. Useful for group-based performance reporting.

Lists all configured groups
- **list_locations**: Useful for auditing site-based workforce distribution.

Lists all configured locations
- **list_people**: Includes names, emails, and internal IDs. Use this to identify personnel before querying their time entries.

Lists all people in the organization
- **list_projects**: Use this when the user asks for a project-based time breakdown.

Lists all configured projects
- **list_time_entries**: Returns employee IDs, entry times, and durations. Use this to monitor workforce activity and total work hours.

Lists all time entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jibble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all people in my Jibble organization."

**🤖 AI Agent:**
> I'll fetch the list of all members in your Jibble organization.

---

**👤 You:**
> "Show me the recent time entries."

**🤖 AI Agent:**
> I'll retrieve the latest time tracking entries from Jibble.

---

**👤 You:**
> "What are the active projects in Jibble?"

**🤖 AI Agent:**
> I'll look up the list of configured projects in your account.


## Installation & Usage

To install and use the **Jibble** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jibble](https://vinkius.com/mcp/jibble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
