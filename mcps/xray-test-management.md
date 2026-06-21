# Xray (Test Management) MCP Server

Manage test cases, executions, and plans on Xray — the leading quality assurance platform for Jira.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/xray-test-management)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Xray Test Management** account to any AI agent and manage your quality assurance workflows through natural conversation.

### What you can do

- **Test Case Discovery** — List and browse all test cases within your project and retrieve unique test keys (e.g., TST-1) for deep inspection
- **Execution Monitoring** — List and track test execution records to monitor real-time QA results and overall release readiness
- **Granular Results** — Retrieve detailed results for specific executions to see which steps passed, failed, or encountered errors
- **Test Planning** — Browse high-level test plans and retrieve scope details to understand your testing strategy and progress
- **Logical Grouping** — List test sets to see how individual test cases are organized into functional or regression groups
- **Historical Auditing** — Retrieve the complete run history for a single test across multiple execution cycles to identify flaky tests
- **Project Config** — Verify environment settings and status mappings to ensure your agent is aligned with your project's workflow

### How it works

1. Subscribe to this server
2. Enter your Xray Client ID and Client Secret
3. Start managing your QA library through Claude, Cursor, or any MCP-compatible client

No more manual filtering through complex Jira issue lists to find a test result. Your AI agent becomes your QA operations analyst.

### Who is this for?

- **QA Engineers** — monitor test execution results and audit test case history through simple chat commands
- **Test Managers** — quickly surface test plan progress and verify test set organization without manual navigation
- **Product Owners** — check the latest execution status before releases to ensure quality standards are met
- **Developers** — lookup test steps and preconditions for failed executions to rapidly debug issues


## Available Tools
- **get_xray_settings**: Retrieves Xray project configuration and field mappings
- **get_execution_details**: Retrieves granular results for a specific test execution
- **get_test_plan_details**: Retrieves details for a specific test plan
- **get_individual_test_runs**: Retrieves individual test run instances for a specific test
- **get_test_details**: Retrieves comprehensive details for a specific Xray test case
- **list_test_executions**: Lists all test execution records
- **list_test_plans**: Lists all test plans configured in Xray
- **list_test_sets**: Lists all test sets (groups of tests)
- **list_xray_tests**: g. TST-1).

Lists all test cases in the Xray project


## Installation & Usage

To install and use the **Xray (Test Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xray-test-management](https://vinkius.com/mcp/xray-test-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
