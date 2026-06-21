# SonarCloud MCP Server

Merge your SaaS DevOps workflow with SonarCloud to review AI code and prevent production vulnerabilities.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sonarcloud)

## Overview
**Category:** ship-it
**Tools Count:** 9

## Description
Bring **SonarCloud’s** industry-leading static code analysis and quality gate checks natively to your AI assistant. Eliminate manual portal checks by querying project bugs, technical debt metrics, and security hotspots dynamically inside your editor via the MCP protocol. Ensure the AI writes secure, compliant data structures aligned with your strict SonarCloud CI/CD definitions.

### What you can do

- **Project Surveillance** — Discover application projects via `search_projects` and fetch internal component hierarchies calling `list_project_components`
- **Vulnerability Hunting** — Expose specific codebase flaws instantly with `search_issues`, extracting actionable remediation steps querying `get_issue_details`
- **Quality Check** — Inspect code passing grades via `get_quality_gate_status` and retrieve specific KPI metrics like coverage using `get_project_measures`
- **Operation Controls** — Pull your organizations (`list_organizations`) and team members (`search_users`) actively tied to specific code repositories

### How it works

1. Subscribe to this AI integration server
2. Introduce your personal SonarCloud Security Token
3. Instruct your local AI assistant to verify project coverage before pushing a PR

Stop digging through the SonarCloud UI just to see why an automated test or quality gate failed. Find the precise faulty dependency versions instantly within your codebase context.

### Who is this for?

- **Software Developers** — request a quick scan check over your latest component before a CI/CD build starts complaining
- **DevSecOps** — query exact details on failing quality gates prior to approving PR merges
- **Team Leads** — gather accurate metrics like lines of code or code coverage directly via textual prompts without opening analytical dashboards


## Available Tools
- **get_issue_details**: Retrieves details for a specific issue
- **get_project_measures**: Requires project key and comma-separated metric keys.

Retrieves quality measures for a specific project component
- **get_analysis_status**: Retrieves the latest analysis status for a project
- **get_quality_gate_status**: g., "OK", "ERROR").

Retrieves the quality gate status for a project
- **list_project_components**: Lists files and directories (components) within a project
- **list_organizations**: Lists organizations for the current user
- **search_issues**: Filter by component (project) key.

Searches for code quality issues
- **search_projects**: You can filter by organization key.

Searches for projects in SonarCloud
- **search_users**: Searches for users in the organization


## Installation & Usage

To install and use the **SonarCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonarcloud](https://vinkius.com/mcp/sonarcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
