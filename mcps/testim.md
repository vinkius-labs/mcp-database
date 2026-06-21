# Testim MCP Server

Trigger automated AI tests, inspect execution logs, and manage branches natively via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/testim)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Testim** project to any AI agent and bring your automated end-to-end testing orchestration directly into your workflow via natural conversation.

### What you can do

- **Automated AI Tests** — Browse your entire test suite, retrieve detailed test steps, and manually trigger specific tests or entire scheduled plans
- **Suite & Label Runs** — Execute dynamic batches by triggering runs associated with specific labels or grouped within precise test suites
- **Execution Diagnostics** — Pull pass/fail statuses, trace errors, and review specific execution logs immediately after a deployment
- **Branch Management** — Check parallel development efforts by listing, creating, and even merging automated test branches without opening the Testim GUI

### How it works

1. Subscribe to this server
2. Enter your Testim Project ID and API Key
3. Command your E2E pipelines straight from Claude, Cursor, or any MCP-compatible platform

### Who is this for?

- **QA Engineers** — trigger full regression test suites via chat as soon as a new environment is ready
- **Frontend Developers** — run specific E2E test scripts right inside their editor IDE (like Cursor) without context switching
- **Release Managers** — rapidly audit the health of test plans and retrieve a specific execution ID to ensure green lights before deploying


## Available Tools
- **create_project_branch**: Creates a new test development branch
- **get_execution_results**: Retrieves the status and results of a specific test execution
- **get_test_details**: Retrieves full details for a specific Testim test
- **list_project_branches**: Lists all parallel development branches in the project
- **list_tests**: Lists all automated tests in the Testim project
- **merge_project_branch**: Typically merges a feature branch into master.

Merges test changes from one branch into another
- **run_tests_by_label**: Triggers a run for all tests matching a specific label
- **run_test_plan**: Triggers a run for a defined test plan
- **run_test_suite**: Triggers a run for all tests in a specific suite
- **run_specific_test**: Optionally provide a branch name. Returns an execution ID.

Triggers an immediate run for a specific test


## Installation & Usage

To install and use the **Testim** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testim](https://vinkius.com/mcp/testim)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
