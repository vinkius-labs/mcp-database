# GUIDEcx MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidecx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guidecx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guidecx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer onboarding via GUIDEcx — manage projects, tasks, and time tracking directly from any AI agent.

## Description
Connect your **GUIDEcx** customer onboarding platform to any AI agent and streamline your implementation workflows through natural conversation.

### What you can do

- **Project Management** — List all onboarding projects, create new implementations, and retrieve detailed status updates.
- **Task Execution** — List tasks across your portfolio, update statuses, and dive into specific task requirements.
- **Team Coordination** — Access lists of users and stakeholders assigned to projects to ensure alignment.
- **Time Tracking** — Log minutes spent on implementation tasks and retrieve time records for reporting.
- **Operational Efficiency** — Use AI to identify overdue tasks or projects that need immediate attention across your entire organization.

### How it works

1. Subscribe to this server
2. Enter your GUIDEcx API Key
3. Start managing your onboarding projects from Claude, Cursor, or any MCP-compatible client

No more manual status updates or digging through project boards. Your AI assistant acts as a proactive implementation manager or project coordinator.

### Who is this for?

- **Implementation Managers** — instantly retrieve project health scores and overdue task lists.
- **Customer Success Teams** — check stakeholder engagement and project milestones directly from the communication flow.
- **Operations Leaders** — automate time record collection and project volume reporting.


## Available Tools
- **create_project**: Create a new onboarding project
- **create_time_record**: Log time against a specific task or project
- **get_project**: Get detailed information about a specific project
- **get_task**: Get details for a specific GUIDEcx task
- **list_project_users**: List stakeholders and users assigned to a specific project
- **list_projects**: List all customer onboarding projects in GUIDEcx
- **list_tasks**: List tasks across projects
- **list_time_records**: List all tracked time records
- **list_users**: List internal organization users
- **update_task**: Update an existing task status or details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GUIDEcx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active onboarding projects."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 4 active implementations: 'Acme Corp Implementation' (ID: 5501), 'Globex Onboarding' (ID: 5505), 'Soylent Corp Setup' (ID: 5510), and 'Initech Rollout' (ID: 5512). Which one would you like to drill down into?

---

**👤 You:**
> "Log 45 minutes for task ID 99283."

**🤖 AI Agent:**
> Time record created! I've successfully logged 45 minutes against task 99283. Would you like to see the updated time report for this project?

---

**👤 You:**
> "Show me the stakeholders for the Acme Corp project."

**🤖 AI Agent:**
> Accessing project users... Stakeholders for 'Acme Corp Implementation' (ID: 5501) include: Robert Paulson (External Lead), Marla Singer (Internal Admin), and Tyler Durden (Project Manager). Shall I list their contact info or assigned tasks?


## Installation & Usage

To install and use the **GUIDEcx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidecx](https://vinkius.com/mcp/guidecx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
