# ChartHop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/charthop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/charthop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/charthop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage people operations and organizational data via ChartHop — track jobs, people, and headcount planning directly from any AI agent.

## Description
Connect your **ChartHop** account to any AI agent and take full control of your organizational data and workforce planning through natural conversation. Streamline how you manage your roster and headcount.

### What you can do

- **Roster Oversight** — List and retrieve details for all people and filled roles in your organization natively
- **Headcount Planning** — Access and monitor open job positions and headcount scenarios flawlessly
- **Organizational Mapping** — List departments, teams, and their hierarchical structures securely
- **Deep-Dive Profiles** — Retrieve complete person information, including job history and compensation metadata flawlessly
- **Scenario Visibility** — Access and review headcount and compensation planning scenarios in real-time
- **System Intelligence** — Retrieve core organization information and account settings directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChartHop API Authorization Token and Org ID
3. Start managing your organization from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **People Ops Managers** — monitor organizational health and review headcount plans using natural language
- **HR Business Partners** — audit department structures and team rosters without opening the dashboard
- **Hiring Managers** — quickly look up open roles and candidate details straight from their chat interface
- **Executives** — verify total headcount and organizational summaries


## Available Tools
- **get_job_details**: Get detailed information for a specific job
- **get_organization_summary**: Retrieve core organization information and settings
- **get_person_details**: Get detailed profile information for a specific person
- **list_organization_departments**: List all departments in the organization
- **list_organization_jobs**: List all jobs (roles) in the organization
- **list_organization_people**: List all people (employees) in the organization
- **list_planning_scenarios**: List headcount and compensation planning scenarios
- **list_organization_teams**: List all teams in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChartHop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the headcount summary for my organization."

**🤖 AI Agent:**
> Retrieving organization summary... You currently have 150 filled roles and 12 open positions across 5 departments. The largest department is Engineering with 65 people.

---

**👤 You:**
> "List all departments and their leaders."

**🤖 AI Agent:**
> Checking departments... I found 5 departments: Engineering (Lead: John Doe), Sales (Lead: Sarah Miller), Marketing (Lead: Mike Scott), Product (Lead: Jane Smith), and HR (Lead: Pam Beesly).

---

**👤 You:**
> "Show me details for 'John Smith' in ChartHop."

**🤖 AI Agent:**
> Searching for 'John Smith'... I found 1 matching profile. John is a 'Senior Software Engineer' in the 'Engineering' department, reporting to 'Jane Smith'. He started on 2022-05-10.


## Installation & Usage

To install and use the **ChartHop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/charthop](https://vinkius.com/mcp/charthop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
