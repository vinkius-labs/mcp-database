# Forecast MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/forecast)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/forecast-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/forecast-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage AI-powered project resources via Forecast — track projects and tasks, handle team availability, and monitor milestones directly from any AI agent.

## Description
Connect your **Forecast.app** account to any AI agent and take full control of your resource management and project scheduling through natural conversation.

### What you can do

- **Project Orchestration** — Retrieve the global array of all managed projects and fetch comprehensive scheduling and resource states belonging to specific project IDs natively
- **Task Lifecycle Auditing** — Enumerate specific physical tasks allocated under project IDs to track work completion and identify bottlenecks synchronously
- **Personnel Oversight** — Fetch physical identity definitions and availability constraints of global members to manage team utilization and workload limits securely
- **Client Relationship Mapping** — Extract explicit client relationships mapped to projects inside your account to manage stakeholder communications flawlessly
- **Milestone Tracking** — Identify timebox markers bounding specific sprint or deliverable targets to ensure project timelines remain within active boundaries
- **Resource Allocation Discovery** — Analyze specific localized variables decoding active assignments and extracting hidden structural constraints across your portfolio
- **Operational Metadata retrieval** — Access global account metadata and project-level attributes to verify workspace configurations natively

### How it works

1. Subscribe to this server
2. Enter your Forecast Personal API Key (found in Forecast > Admin > API Keys)
3. Start managing your project resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers & Leads** — track task progress and team availability without manual status updates
- **Resource Coordinators** — audit team utilization and manage member workloads using natural language conversation
- **Operations Teams** — monitor project milestones and verify client-project relationships in real-time
- **Developers** — test and debug resource management integrations and verify task schemas through the chat interface


## Available Tools
- **list_projects**: List projects
- **get_project**: Get project details
- **list_tasks**: List tasks
- **list_people**: List people
- **list_clients**: List clients
- **list_milestones**: List milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Forecast"

**🤖 AI Agent:**
> Retrieving projects... I found 5 active projects: 'Q2 Marketing Launch', 'API V2 Development', 'Client Dashboard Refactor', 'Security Audit', and 'New Website Build'. Which one would you like to see the tasks for?

---

**👤 You:**
> "Show me the tasks for project 'API V2 Development'"

**🤖 AI Agent:**
> Retrieving tasks for 'API V2 Development' (ID: 123)... I found 10 tasks including 'Define Auth Schema' (In Progress), 'Implement Webhooks' (Todo), and 'Rate Limiting Logic' (Done). Would you like to see the assignee for the auth schema task?

---

**👤 You:**
> "Who is available this week for a new assignment?"

**🤖 AI Agent:**
> Checking team availability... John and Sarah have 10+ hours of open capacity this week. Mike and Alice are currently fully booked on the Marketing project. Would you like me to assign a new task to Sarah?


## Installation & Usage

To install and use the **Forecast** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forecast](https://vinkius.com/mcp/forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
