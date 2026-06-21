# Zephyr Scale (SmartBear) MCP Server

Manage test cases, cycles, and executions on Zephyr Scale — the high-performance test management tool for Jira.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zephyr-scale-smartbear)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Zephyr Scale (SmartBear)** account to any AI agent and manage your enterprise quality assurance infrastructure through natural conversation.

### What you can do

- **Test Case Discovery** — List and browse all test cases within a Jira project and retrieve specific keys (e.g., PROJ-T1) for deep inspection
- **Cycle Monitoring** — Browse test cycles to see how test runs are grouped for specific releases, sprints, or regression cycles
- **Execution Tracking** — Monitor real-time test execution results (Pass, Fail, Blocked) and retrieve step-by-step progress details
- **Test Planning** — List high-level test plans to understand your overall testing strategy and project scope
- **Folder Navigation** — Explore the organizational hierarchy of your test cases, cycles, and plans to find specific work items
- **Environment Audit** — List configured test environments (Staging, Production) and custom statuses available for your project
- **Step-by-Step Insights** — Retrieve full objective, preconditions, and detailed test scripts for any individual test case

### How it works

1. Subscribe to this server
2. Enter your Zephyr Scale API Token
3. Start managing your QA cycles through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex Jira plugins to find a test script. Your AI agent becomes your QA operations coordinator.

### Who is this for?

- **QA Engineers** — monitor test execution results and audit test case scripts through simple chat commands
- **Test Managers** — quickly surface test cycle progress and verify test plan organization without manual filtering
- **Release Managers** — check the execution status of regression cycles before approving production deployments
- **Developers** — lookup test steps and preconditions for failed executions to rapidly debug software defects


## Available Tools
- **get_execution**: Retrieves full details of a Zephyr Scale test execution
- **list_test_plans**: Lists all test plans in a Zephyr Scale project
- **list_test_cases**: Provide a Jira project key (e.g. "PROJ"). Returns test case keys, names, and statuses. Paginated.

Lists all test cases in a Zephyr Scale project
- **get_test_case**: Retrieves full details of a Zephyr Scale test case
- **list_test_cycles**: Test cycles group test runs for a release or sprint.

Lists all test cycles in a Zephyr Scale project
- **get_test_cycle**: Retrieves full details of a Zephyr Scale test cycle
- **list_executions**: Lists all test executions in a Zephyr Scale project
- **list_folders**: Folder type must be TEST_CASE, TEST_CYCLE, or TEST_PLAN.

Lists all folders for a specific type within a project
- **list_statuses**: Lists all custom test execution statuses in a project
- **list_environments**: g. Staging, Production).

Lists all test environments in a Zephyr Scale project


## Installation & Usage

To install and use the **Zephyr Scale (SmartBear)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zephyr-scale-smartbear](https://vinkius.com/mcp/zephyr-scale-smartbear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
