# TestLink MCP Server

Navigate your self-hosted TestLink instance to inspect test plans, suites, cases, and builds natively via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/testlink)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **TestLink** self-hosted environment to any AI agent and bring your classic test management structure seamlessly into your modern AI workflow via natural language.

### What you can do

- **Project & Plan Scoping** — Retrieve all test projects, query their active states, and list all comprehensive test plans linked to them
- **Suite Navigation** — Browse the hierarchical folder tree of Test Suites mapping your organizational test coverage
- **Test Cases Verification** — Dive deep into individual test cases to read manual steps, expected results, priorities, and preconditions without navigating the legacy UI
- **Build Tracking** — Inspect active software builds allocated within any specific test plan to confirm QA target versions
- **Environment Sanity** — Check the agent’s connection and user mapping via the native whoami interrogation

### How it works

1. Subscribe to this server
2. Enter your instance Base URL and Developer API Key
3. Start querying test protocols and scopes from Claude, Cursor, or any MCP-compatible platform

### Who is this for?

- **QA Leads** — pull test plans and historical cases into chat seamlessly when defining regression cycles
- **Test Engineers** — recall specific step-by-step instructions from legacy cases into their markdown editors
- **Developers** — verify the preconditions and expected results of a highly complex bug without requesting UI access from QA


## Available Tools
- **get_test_case_details**: Retrieves full details for a specific test case
- **get_test_plan_details**: Retrieves details for a specific test plan
- **get_test_project_details**: Retrieves details for a specific TestLink test project
- **get_test_suite_details**: Retrieves details for a specific test suite
- **list_test_builds**: Lists all builds available for a specific test plan
- **list_test_cases**: Lists all test cases within a specific test suite
- **list_test_plans**: Requires a project ID.

Lists all test plans associated with a specific project
- **list_test_projects**: Lists all test projects available on the TestLink server
- **list_test_suites**: Lists all test suites within a specific test project
- **get_user_info**: Retrieves information about the authenticated TestLink user


## Installation & Usage

To install and use the **TestLink** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testlink](https://vinkius.com/mcp/testlink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
