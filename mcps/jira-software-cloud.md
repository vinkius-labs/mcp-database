# Jira Software Cloud MCP Server

Manage Jira Software Agile workflows — list boards, track sprints, manage backlogs, and inspect epics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jira-software-cloud)

## Overview
**Category:** industry-titans
**Tools Count:** 31

## Description
Connect your **Jira Software Cloud** instance to any AI agent to streamline your Agile project management. This server provides deep integration with Jira's Software-specific features like Boards, Sprints, and Epics.

### What you can do

- **Board Management** — List all Scrum and Kanban boards, fetch their configurations, and view associated Sprints or Epics.
- **Sprint Control** — Create new sprints, retrieve sprint details, and update sprint states (start or complete) to keep your team moving.
- **Backlog & Issues** — Query board backlogs, fetch issues within specific sprints or epics, and manage issue rankings.
- **Estimation Tracking** — Retrieve and set story point estimations for agile issues to maintain velocity visibility.
- **DevOps Integration** — Submit and query development information including builds, deployments, and feature flags.

### How it works

1. Subscribe to this server
2. Provide your Jira Domain, Email, and API Token
3. Start managing your sprints and boards from Claude, Cursor, or any MCP client

### Who is this for?

- **Scrum Masters & PMs** — Quickly check sprint progress, move issues, and update sprint statuses without the heavy Jira UI.
- **Developers** — Check backlog priorities and update estimations directly from your coding environment.
- **Release Managers** — Track builds and deployments associated with Jira issues in real-time.


## Available Tools
- **create_board**: Requires name, type (scrum or kanban), and filterId.

Create a new board
- **create_sprint**: Create a new sprint
- **get_agile_issue**: Get issue with Agile fields
- **get_board_backlog**: Get issues for backlog
- **get_board_configuration**: Get board configuration
- **get_board_epics**: Get all epics for board
- **get_board_sprints**: Get all sprints for board
- **get_build**: Get build data
- **get_deployment_gating_status**: Get deployment gating status
- **get_epic_issues**: Get issues for epic
- **get_epic**: Get epic details
- **get_issue_estimation**: Get issue estimation
- **get_repository_dev_info**: Get repository development information
- **get_sprint_issues**: Get issues for sprint
- **get_sprint**: Get sprint details
- **link_security_workspaces**: Link security workspaces
- **list_boards**: Get all boards in Jira Software
- **move_issues_to_backlog**: Move issues to backlog
- **move_issues_to_epic**: Move issues to epic
- **move_issues_to_sprint**: Move issues to sprint
- **rank_epics**: Rank epics
- **rank_issues**: Rank issues
- **set_issue_estimation**: Set issue estimation
- **store_dev_info**: Store development information
- **submit_builds**: Submit build data
- **submit_deployments**: Submit deployment data
- **submit_feature_flags**: Submit feature flag data
- **submit_incidents**: Submit incidents or reviews
- **submit_remote_links**: Submit remote link data
- **submit_vulnerabilities**: Submit vulnerabilities
- **update_sprint**: Can be used to start or complete a sprint by changing state to active or closed.

Update a sprint


## Installation & Usage

To install and use the **Jira Software Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jira-software-cloud](https://vinkius.com/mcp/jira-software-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
