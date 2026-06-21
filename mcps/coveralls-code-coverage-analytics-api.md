# Coveralls (Code Coverage Analytics API) MCP Server

Track code coverage metrics via Coveralls — manage repositories, submit coverage reports, and monitor build statuses directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coveralls-code-coverage-analytics-api)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Coveralls** account to any AI agent to streamline your CI/CD workflows and maintain high code quality standards through natural conversation.

### What you can do

- **Repository Management** — Create, retrieve, and update repository configurations and access tokens across GitHub, GitLab, and Bitbucket
- **Coverage Submission** — Submit detailed coverage reports (jobs) including source file data and git metadata directly to the Coveralls API
- **Parallel Build Control** — Manage complex parallel CI workflows by triggering final aggregate calculations and closing build sequences
- **Build Reruns** — Quickly trigger a rerun of build processing to resolve transient issues without manual dashboard intervention
- **Web Data Insights** — Fetch JSON representations of repository and build pages to analyze recent trends and coverage history

### How it works

1. Subscribe to this server
2. Enter your Coveralls Personal Access Token
3. Start monitoring your code quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the setup of new repositories and monitor coverage trends across the organization
- **Software Developers** — check coverage status and submit reports directly from the terminal or IDE
- **QA Leads** — analyze coverage regressions and manage build thresholds to ensure code reliability


## Available Tools
- **close_parallel_build**: Close a parallel build on Coveralls
- **create_repo**: Requires personal API token.

Create a new repository on Coveralls
- **get_build_web_data**: May require personal API token for private repos.

Get JSON representation of a build web page
- **get_file_web_data**: May require personal API token for private repos.

Get JSON representation of a source file web page
- **get_job_web_data**: May require personal API token for private repos.

Get JSON representation of a job web page
- **get_repo**: Requires personal API token.

Get repository info from Coveralls
- **get_repo_web_data**: May require personal API token for private repos.

Get JSON representation of a repo web page
- **rerun_build**: Trigger a rerun of a build on Coveralls
- **submit_job**: Requires repo_token, service_name, service_job_id, source_files, and git metadata.

Submit a coverage report (job) to Coveralls
- **update_repo**: Requires personal API token.

Update an existing repository on Coveralls


## Installation & Usage

To install and use the **Coveralls (Code Coverage Analytics API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coveralls-code-coverage-analytics-api](https://vinkius.com/mcp/coveralls-code-coverage-analytics-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
