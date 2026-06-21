# TestMonitor MCP Server

List QA projects, extract test runs, read user assignments, and fetch tracked issues strictly from your AI chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/testmonitor)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Link up your **TestMonitor** cloud infrastructure with any AI agent to streamline QA tracking operations and retrieve real-time milestone data without having to navigate web dashboards.

### What you can do

- **Project Triage** — List all ongoing projects alongside their high-level metadata such as test coverage and delivery status
- **Runs & Milestones Tracking** — Instantly retrieve project-scoped test runs, milestones lists, and deadline progress
- **Defect Auditing** — Query all generated issues or software defects explicitly linked to a specific test project
- **Requirement Tracing** — Ask the agent to map requirements against existing feature specifications without manually matching them in the UI
- **Team Management Lookup** — Easily list out all the users provisioned in the workspace to confirm roles or debugging ownership

### How it works

1. Subscribe to this server
2. Provide your Subdomain and your Personal Access Token
3. Coordinate your entire QA suite from Claude, Cursor, or any compatible AI IDE

### Who is this for?

- **Quality Directors** — request a quick summary of the current Test Runs and their respective Milestones before daily stand-ups
- **Bug Triagers** — leverage the AI to list reported defects and quickly assign the contextual backlog data to new tickets
- **Product Owners** — read the explicit specifications of any Requirement and cross-reference against active test cases without breaking focus


## Available Tools
- **get_test_case_details**: Retrieves full details for a specific TestMonitor test case
- **get_project_details**: Retrieves details for a specific TestMonitor project
- **get_test_run_details**: Retrieves details for a specific TestMonitor test run
- **list_test_cases**: Lists all test cases within a specific TestMonitor project
- **list_issues**: Lists all issues (defects) within a project
- **list_milestones**: Lists all milestones within a project
- **list_projects**: Project IDs are required for most other tools.

Lists all projects available on the TestMonitor instance
- **list_requirements**: Lists all requirements for a project
- **list_test_runs**: Lists all test runs within a specific project
- **list_account_users**: Lists all users associated with the TestMonitor account


## Installation & Usage

To install and use the **TestMonitor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testmonitor](https://vinkius.com/mcp/testmonitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
