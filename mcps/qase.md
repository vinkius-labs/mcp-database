# Qase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Bring Qase test management into your AI workflow — list projects, track test runs, inspect cases, and monitor defects directly from your chat.

## Description
Connect your **Qase** workspace to any AI agent and integrate test management deeply into your development workflow.

### What you can do

- **Project Overviews** — Retrieve all active projects, view health metrics, and get total counts of test cases, runs, and defects instantly
- **Test Cases & Suites** — Explore your test hierarchy, pull specific test steps, and check case automation statuses without opening the Qase dashboard
- **Test Runs & Execution** — List all test runs, monitor execution status (passed, failed, blocked), and dive deep into test run analytics
- **Defects & Milestones** — Track project milestones and extract all logged defects linked to failed test cases, complete with severity levels and issue links

### How it works

1. Subscribe to this server
2. Authorize via your Qase API Token
3. Start managing QA operations directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — quickly pull up test case steps while writing automated scripts in your IDE
- **Developers** — ask your agent to list recent defects or failed runs related to the feature you just deployed
- **Product Managers** — get instant summaries of test run coverage and milestone completion metrics


## Available Tools
- **list_projects**: Lists all projects in Qase
- **get_project**: Retrieves details for a specific project
- **list_cases**: Lists test cases in a project
- **get_case**: Retrieves details for a specific test case
- **list_suites**: Lists test suites in a project
- **list_runs**: Lists all test runs in a project
- **get_run**: Retrieves details for a specific test run
- **list_plans**: Lists all test plans in a project
- **list_milestones**: Lists all milestones in a project
- **list_defects**: Lists all defects linked to test case failures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Qase projects and show me their overall health."

**🤖 AI Agent:**
> I retrieved 3 active projects in your Qase instance. 
1. Mobile App (Code: MOB) - 150 test cases, 3 active open defects.
2. Web Portal (Code: WEB) - 300 test cases, 12 test runs.
3. API V2 (Code: API) - 50 test cases, 0 defects.
Should I inspect the defects on the Mobile App project?

---

**👤 You:**
> "Fetch the details of test case ID 45 in the WEB project."

**🤖 AI Agent:**
> Here are the details for WEB-45 ('User Login using SSO'):
- Pre-conditions: User must have an active Google SSO account.
- Step 1: Click 'Login with Google' - Expected: Google Auth modal opens.
- Step 2: Enter valid credentials - Expected: Redirect to dashboard.
Shall I write a Cypress test for this?

---

**👤 You:**
> "Are there any recent defects added for the WEB project?"

**🤖 AI Agent:**
> Yes, I queried the `list_defects` capability. There are 2 new defects recorded today:
1. Defect #11: 'CSS layout breaks on mobile' (Severity: High)
2. Defect #12: 'API timeout during checkout' (Severity: Critical)
Both are in 'open' status. Shall I pull the details for #12?


## Installation & Usage

To install and use the **Qase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qase](https://vinkius.com/mcp/qase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
