# Codecov MCP Server

Manage test coverage and engineering metrics via Codecov — track coverage reports, monitor commit totals, and audit code quality directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/codecov)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **Codecov** account to any AI agent and take full control of your test coverage and engineering insights through natural conversation. Streamline how you monitor software quality across your repositories natively.

### What you can do

- **Repository Oversight** — List and retrieve details for all repositories including their current coverage percentage natively
- **Commit Intelligence** — Access aggregate coverage totals for specific commit SHAs to verify build health flawlessly
- **Report Hierarchy** — Retrieve a hierarchical view of coverage reports matching your project's file structure flawlessly
- **Branch & Flag Logistics** — Monitor coverage across different branches and custom flags to understand distribution securely
- **Developer Insights** — Access your own user profile and core account metadata directly within your workspace flawlessly
- **integrated Visibility** — Retrieve detailed repository metadata including service provider and owner information flawlessly

### How it works

1. Subscribe to this server
2. Enter your Codecov Global API Token (obtained from Settings > Access)
3. Start managing your test coverage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — monitor coverage changes and audit specific file reports using natural language
- **Engineering Managers** — review team coverage trends and repository health without opening the dashboard
- **DevOps Engineers** — quickly look up commit coverage totals and verify build status straight from their chat interface
- **Quality Assurance** — verify test completeness and monitor coverage flags across platforms


## Available Tools
- **get_commit_coverage_totals**: Retrieve aggregate coverage totals for a specific commit SHA
- **get_my_codecov_profile**: Retrieve information about the authenticated user
- **get_repository_coverage_details**: Get detailed coverage information for a specific repository
- **get_coverage_report_tree**: Retrieve a hierarchical view of the coverage report matching the file structure
- **list_repository_branches**: List all branches tracked in Codecov
- **list_repository_commits**: List recent commits and their coverage status
- **list_coverage_flags**: List all coverage flags defined for a repository
- **list_codecov_repositories**: List all repositories associated with an owner


## Installation & Usage

To install and use the **Codecov** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codecov](https://vinkius.com/mcp/codecov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
