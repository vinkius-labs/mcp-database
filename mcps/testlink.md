# TestLink MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/testlink)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/testlink-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/testlink-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Navigate your self-hosted TestLink instance to inspect test plans, suites, cases, and builds natively via your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TestLink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find out if the server is working and tell me who I am authenticated as."

**🤖 AI Agent:**
> Server is reachable! The token is authenticating as user `QA_Admin` on project footprint ID `1`. How can I assist you with your QA coverage today?

---

**👤 You:**
> "Give me the step-by-step definition for Test Case ID 5440."

**🤖 AI Agent:**
> Here are the details for Test Case 'Billing Module Crash' (ID 5440):
- **Preconditions**: User must have a cart with exactly $0 in amount.
- **Step 1**: Attempt to proceed to checkout bypassing frontend validation using cURL. (Expected: 400 Bad Request error returned).
- **Step 2**: Open Stripe gateway page. (Expected: Page throws exception cleanly).
Would you like me to flag this into an exportable markdown table?

---

**👤 You:**
> "List all active test plans for Project ID 2."

**🤖 AI Agent:**
> I found 2 active test plans mapped directly to Project ID 2:
1. 'Release v1.5 - Regression Sandbox' (Plan ID: 1045)
2. 'Payment Gateway E2E' (Plan ID: 1993)
Which plan would you like to retrieve the registered builds for?


## Installation & Usage

To install and use the **TestLink** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testlink](https://vinkius.com/mcp/testlink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
