# TestRail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/testrail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/testrail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/testrail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Browse TestRail suites, parse manual test specs, and monitor active runs seamlessly native within your conversational AI workflow.

## Description
Bring your overarching **TestRail** quality assurance orchestration directly to your developer's edge. Query comprehensive test coverage, inspect failing builds, and extract explicit test steps using natural conversation.

### What you can do

- **Project Triage** — Extract active test projects, their numeric IDs, and overall suite architecture logic
- **Suite & Case Isolation** — Retrieve precise step-by-step logic, preconditions, and validation targets for any manual test case stored by QA
- **Run Execution Metrics** — Instantly generate summaries around active 'Test Runs', seeing precisely which specific tests passed or failed
- **Milestone Navigation** — Interrogate upcoming QA deadlines and release milestones without ever touching the heavy web browser application
- **Deep Hierarchical Search** — Pull Section lists (folder hierarchies) from within projects to navigate robust test repositories visually in markdown

### How it works

1. Subscribe to this server
2. Provide your TestRail Base URL alongside your authenticated Email & API Key
3. Start fetching and aggregating QA metrics from Claude, Cursor, or any MCP-oriented platform

### Who is this for?

- **Test Leads** — generate immediate health summaries of active Milestones and Test Runs without digging into dashboard tables
- **Software Devs** — pull down manual reproduction steps natively inside Cursor IDE to fix bugs without switching screens
- **Automation Engineers** — analyze the properties of 'Test Cases' to rapidly convert them into code-based e2e automated tests


## Available Tools
- **get_test_case_details**: Retrieves full details for a specific test case
- **get_test_project_details**: Retrieves details for a specific TestRail project
- **get_test_run_details**: Retrieves details for a specific test run
- **list_test_cases**: Lists all test cases in a project, optionally filtered by suite
- **list_project_milestones**: Lists all milestones within a project
- **list_test_projects**: Project IDs are essential for navigating most other resources.

Lists all test projects available on the TestRail instance
- **list_test_runs**: Lists all test runs within a specific project
- **list_project_sections**: Lists all sections (folders) within a project
- **list_test_suites**: Lists all test suites within a specific project
- **list_run_tests**: Lists all tests (case instances) within a specific test run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TestRail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What active TestRail projects are available in this instance?"

**🤖 AI Agent:**
> Found 2 active TestRail projects:
- **`ID: 15`** | "Native Mobile Apps (Q2)" | Uses standard multi-suite mode.
- **`ID: 29`** | "Core Payment Backend" | Single suite repository.
Should I list milestones or test suites under Project ID 15?

---

**👤 You:**
> "Get the manual preconditions and test steps for Test Case 1285."

**🤖 AI Agent:**
> Case ID `1285`: **OAuth Registration Gateway Failure**
> **Priority:** CRITICAL_HIGH | **Estimate:** 5m
> **Preconditions:** Server must be isolated via VPN routing rules.

**Steps:**
1. Call initialization endpoint bypassing token assignment. (Expected Result: API triggers `ERR401` gracefully without cascading stack traces).
2. Force brute-force retries mimicking scripts. (Expected Result: IP locks completely after exactly 5th try).
Can I translate these rules over towards a framework structure?

---

**👤 You:**
> "Return exact status summary for Test Run ID 403."

**🤖 AI Agent:**
> Metrics recovered for Test Run **`#403: Sanity Validation Build.v45`**:
- **Total Executed Tests:** 80
- **Passed:** 71 ✅
- **Failed (Action Required):** 6 ❌
- **Blocked (Dependency issues):** 3 ⏸️
This run has notable defect traces. Would you like me to extract the exact test lists behind the 6 failed triggers?


## Installation & Usage

To install and use the **TestRail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testrail](https://vinkius.com/mcp/testrail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
