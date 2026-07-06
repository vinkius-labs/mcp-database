# Zephyr Scale (SmartBear) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zephyr-scale-smartbear)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage test cases, cycles, and executions on Zephyr Scale — the high-performance test management tool for Jira.

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


## Available Tools (10)
- **get_execution**: Retrieves full details of a Zephyr Scale test execution
- **get_test_case**: Retrieves full details of a Zephyr Scale test case
- **list_test_cycles**: Test cycles group test runs for a release or sprint.

Lists all test cycles in a Zephyr Scale project
- **get_test_cycle**: Retrieves full details of a Zephyr Scale test cycle
- **list_executions**: Lists all test executions in a Zephyr Scale project
- **list_test_cases**: Provide a Jira project key (e.g. "PROJ"). Returns test case keys, names, and statuses. Paginated.

Lists all test cases in a Zephyr Scale project
- **list_test_plans**: Lists all test plans in a Zephyr Scale project
- **list_folders**: Folder type must be TEST_CASE, TEST_CYCLE, or TEST_PLAN.

Lists all folders for a specific type within a project
- **list_statuses**: Lists all custom test execution statuses in a project
- **list_environments**: g. Staging, Production).

Lists all test environments in a Zephyr Scale project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zephyr Scale (SmartBear)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all test cases in project 'PROJ'."

**🤖 AI Agent:**
> I found 12 test cases in project PROJ. The most recent are: 1. 'User Login' (Key: PROJ-T1), 2. 'Password Reset' (Key: PROJ-T2), and 3. 'Profile Update' (Key: PROJ-T3). Which one would you like to inspect?

---

**👤 You:**
> "What are the details for test cycle 'PROJ-R42'?"

**🤖 AI Agent:**
> Cycle 'PROJ-R42' (Regression Q1): Status: In Progress, Planned Start: 2026-03-25, Planned End: 2026-04-05. It contains 25 test executions. Current progress: 15/25 complete.

---

**👤 You:**
> "Show me the results for execution ID '12345678'."

**🤖 AI Agent:**
> Execution 12345678 Result: FAILED. Total steps: 5. Steps 1-3 Passed, Step 4 Failed: 'Clicking submit button returned no response'. Time taken: 45s. Would you like me to pull the linked Jira issue?


## ❓ FAQ

**Q: Can I check the specific test steps for a case through the agent?**
Yes. The `get_test_case` tool allows your AI agent to retrieve the full script for any test key, providing the exact sequence of steps, test data, and expected results defined in Zephyr Scale.

**Q: How do I see the progress of a specific test cycle via chat?**
Use the `get_test_cycle` tool. Provide the unique cycle key, and your agent will return the cycle status, planned dates, and high-level execution statistics to help you monitor testing progress.

**Q: Is it possible to see the results of individual test runs?**
Absolutely. Using the `get_execution_details` tool, your agent can retrieve step-by-step results for any execution, including comments and execution time, helping you identify exactly where a test failed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zephyr-scale-smartbear](https://vinkius.com/mcp/zephyr-scale-smartbear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zephyr Scale (SmartBear)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zephyr-scale-smartbear` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zephyr Scale (SmartBear)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zephyr-scale-smartbear": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
