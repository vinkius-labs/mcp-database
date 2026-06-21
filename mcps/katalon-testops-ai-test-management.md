# Katalon TestOps (AI Test Management) MCP Server

Manage test orchestration via Katalon TestOps — rerun test runs, monitor execution results, and audit software releases.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/katalon-testops-ai-test-management)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Connect your **Katalon TestOps** account to any AI agent and take full control of your AI-powered test management and quality orchestration through natural conversation.

### What you can do

- **Execution Orchestration** — List all test runs and trigger immediate re-executions of specific suites to verify bug fixes directly from your agent
- **Quality Analytics** — Retrieve detailed test outcome summaries, including pass/fail rates, execution durations, and error stack traces
- **Diagnostic Inspection** — Deep-dive into individual test results to extract application logs, error messages, and visual screenshots for rapid debugging
- **Environment Audit** — List configured execution environments to understand target OS, browser, and device distributions across your projects
- **Release Management** — Monitor defined software releases and track aggregated test run statistics to ensure build quality before deployment
- **Project CRM** — Navigate across multiple Katalon projects and retrieve detailed metadata including team assignments and suite counts securely

### How it works

1. Subscribe to this server
2. Enter your Katalon Email and API Key
3. Start managing your test orchestration from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — monitor release readiness and track team testing progress through natural conversation without jumping between projects
- **Automation Engineers** — rerun failed test suites and inspect diagnostic logs directly from your workspace for rapid iteration
- **DevOps Engineers** — audit execution environments and verify build quality results to ensure CI/CD pipeline integrity


## Available Tools
- **list_projects**: Returns project names, IDs, and descriptions.

List all projects on Katalon TestOps
- **get_project**: Get full details of a Katalon project
- **list_test_runs**: Returns run IDs, pass/fail status, total counts, and execution durations.

List test runs within a Katalon project
- **get_test_run**: Get full details of a Katalon test run
- **rerun_test_run**: Returns the newly created test run ID.

Re-run an existing Katalon test run
- **list_test_results**: Returns durations, statuses, and error messages.

List detailed test results within a test run
- **get_test_result**: Get full details of a single Katalon test result
- **list_execution_environments**: List execution environments in a Katalon project
- **list_project_releases**: Returns release names, scheduled dates, and aggregated test run statistics.

List defined releases in a Katalon project
- **list_project_builds**: Returns build identifier names, IDs, and the count of associated test runs.

List software builds in a Katalon project


## Installation & Usage

To install and use the **Katalon TestOps (AI Test Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/katalon-testops-ai-test-management](https://vinkius.com/mcp/katalon-testops-ai-test-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
