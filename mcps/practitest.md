# PractiTest MCP Server

Bring your end-to-end QA management to your AI — list tests, instances, test sets, requirements, and trace logical software defects natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/practitest)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **PractiTest** workspaces to any AI agent and empower it to orchestrate the entire QA lifecycle from physical requirements tracing to defect mapping natively via chat conversations.

### What you can do

- **Test Cases & Sets** — Tell the AI to investigate any Test Case or Test Set, discovering exact preconditions and expected results (`list_tests`, `get_test`, `list_sets`)
- **Test Instances & Runs** — Retrieve deep execution histories pinpointing exactly which step caused a regression bounding PASSED/FAILED statuses (`list_runs`)
- **Requirements Tracking** — Audit physical system compliance extracting arrays dictating QA delivery thresholds (`list_requirements`)
- **Issue Mapping** — Find exact Software Defects bound natively to QA traces verifying complex failure logic (`list_issues`)

### How it works

1. Subscribe to this server
2. Supply your PractiTest Personal API Token and Project ID
3. Launch Claude, Cursor, or any compatible MCP client to instruct the AI with full test management autonomy

Forget moving between dashboard views trying to identify where a trace broke down. Simply ask the agent 'Why did the latest Payment flow fail?'

### Who is this for?

- **QA Automation Engineers** — verify integration outputs traversing test run histories instantaneously
- **Product Owners** — read live requirement statuses cross-referencing execution states mapped in the chat window
- **Software Developers** — dive into reported Issues parsing exact test execution failures natively before diving into code


## Available Tools
- **list_tests**: List all test cases in a PractiTest project. PractiTest is an end-to-end test management platform with traceability from requirements to defects. Returns test names, IDs, statuses, custom fields, and traceability links. Uses JSON:API format
- **get_test**: Get full details of a PractiTest test case including name, description, preconditions, steps, expected results, custom fields, and requirement links
- **list_sets**: List all test sets in a PractiTest project. Test sets group test instances for execution. Returns set names, statuses, planned/actual dates, and assigned testers
- **get_set**: Get full details of a PractiTest test set including name, status, instances count, and execution summary
- **list_instances**: List all test instances in a PractiTest test set. Instances are test-set-specific copies of test cases. Returns instance IDs, test references, and last run statuses
- **list_runs**: List all runs for a PractiTest test instance. Runs record actual test execution results. Returns run IDs, statuses (PASSED/FAILED/BLOCKED/NOT_RUN/N_A), durations, and timestamps
- **list_requirements**: List all requirements in a PractiTest project. Requirements provide traceability to test cases and defects. Returns names, statuses, and linked test counts
- **list_issues**: List all issues (defects) in a PractiTest project. Returns issue names, statuses, severities, and linked test references
- **list_custom_fields**: List all custom fields in a PractiTest project. Returns field names, types, applicable entities, and possible values
- **list_users**: List all users in the PractiTest account. Returns user names, emails, roles, and statuses


## Installation & Usage

To install and use the **PractiTest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/practitest](https://vinkius.com/mcp/practitest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
