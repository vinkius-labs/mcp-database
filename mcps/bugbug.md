# BugBug MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugbug)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test your web application automatically with no-code browser tests that catch regressions before your users do.

## Description
Connect your **BugBug** account to any AI agent and take full control of your automated browser testing and application quality monitoring through natural conversation.

### What you can do

- **Test Orchestration** — List and run high-fidelity automated browser tests in the cloud programmatically, including support for custom environment IDs
- **Suite Execution Architecture** — Trigger entire test suites to run simultaneously and monitor their aggregate results to oversee platform-wide quality in real-time
- **Run Intelligence** — Retrieve detailed high-fidelity reports and execution status for every test run to identify regressions and friction points instantly
- **History & Performance Monitoring** — Access complete historical records of past test and suite runs to coordinate your QA trends programmatically
- **Infrastructure Visibility** — Access high-fidelity metadata for your projects and retrieve BugBug IP addresses for secure firewall allowlisting directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your BugBug dashboard (Integrations tab)
3. Start automating your QA pipeline from Claude, Cursor, or any MCP client

No more manual triggering of cloud tests or digging through complex run logs. Your AI acts as your dedicated QA engineer and quality architect.

### Who is this for?

- **QA Engineers** — instantly trigger regression suites and retrieve results using natural language commands
- **Developers** — verify application quality after a deployment without leaving your creative workspace
- **DevOps Teams** — automate the retrieval of testing IPs and monitor suite performance through simple AI queries


## Available Tools (12)
- **get_ips**: Get BugBug IP addresses
- **get_suite_run**: Get status of a suite run
- **get_suite**: Get details for a specific suite
- **get_test_run**: Get status of a test run
- **get_test**: Get details for a specific test
- **list_projects**: List all projects
- **list_suite_runs**: List recent suite runs
- **list_suites**: List all test suites
- **list_test_runs**: List recent test runs
- **list_tests**: List all tests
- **run_suite**: Run a specific test suite
- **run_test**: Run a specific test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BugBug** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my automated tests in BugBug."

**🤖 AI Agent:**
> I've retrieved your test directory. You currently have 15 automated tests, including 'Login Flow' (ID: test_123) and 'Checkout Process'. Which one would you like to execute or inspect?

---

**👤 You:**
> "Run the 'Smoke Test' suite (ID: 'suite_456') in the 'Staging' environment."

**🤖 AI Agent:**
> Suite execution triggered! I've initiated the 'Smoke Test' suite in your staging environment. The run ID is 'run_789'. I'll monitor the progress and notify you as soon as the results are ready.

---

**👤 You:**
> "Show the status and results for the latest test run ID 'run_789'."

**🤖 AI Agent:**
> Fetching run results... Execution run_789 has successfully 'Passed'. All 5 steps were verified. You can view the full high-fidelity report here: [report_url]. Shall I check the historical trends for this test?


## ❓ FAQ

**Q: How do I find my BugBug API Token?**
Log in to your account, navigate to the **Integrations** tab in the sidebar, and copy your unique API Token.

**Q: Can I run tests in a specific environment?**
Yes! Both `run_test` and `run_suite` tools accept an optional `environmentId` parameter to target specific deployment stages.

**Q: How do I get the IP addresses for allowlisting?**
Use the `get_ips` tool to retrieve the list of high-fidelity IP addresses used by BugBug's cloud infrastructure programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugbug](https://vinkius.com/mcp/bugbug)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BugBug** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bugbug` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BugBug** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bugbug": {
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
