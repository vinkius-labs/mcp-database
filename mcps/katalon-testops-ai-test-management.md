# Katalon TestOps (AI Test Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/katalon-testops-ai-test-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage test orchestration via Katalon TestOps — rerun test runs, monitor execution results, and audit software releases.

## Description
Connect your **Katalon TestOps** account to any AI agent and take full control of your AI-powered test management and quality orchestration through natural conversation.

### What you can do

- **Execution Orchestration** — List all test runs and trigger immediate re-executions of specific suites to verify bug fixes directly from your agent
- **Quality Analytics** — Retrieve detailed test outcome summaries, including pass/fail rates, execution durations, and error stack traces
- **Diagnostic Inspection** — Deep-dive into individual test results to extract application logs, error messages, and visual screenshots for rapid debugging
- **Environment Audit** — List configured execution environments to understand target OS, browser, and device distributions across your projects
- **Release Management** — Monitor defined software releases and track aggregated test run statistics to ensure build quality before deployment
- **Project CRM** — Navigate across multiple Katalon projects and retrieve detailed metadata including team assignments and suite counts securely

### How it works

1. Subscribe to this server
2. Enter your Katalon Email and API Key
3. Start managing your test orchestration from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — monitor release readiness and track team testing progress through natural conversation without jumping between projects
- **Automation Engineers** — rerun failed test suites and inspect diagnostic logs directly from your workspace for rapid iteration
- **DevOps Engineers** — audit execution environments and verify build quality results to ensure CI/CD pipeline integrity


## Available Tools
- **list_projects**: Returns project names, IDs, and descriptions.

List all projects on Katalon TestOps
- **get_project**: Get full details of a Katalon project
- **list_test_runs**: Returns run IDs, pass/fail status, total counts, and execution durations.

List test runs within a Katalon project
- **get_test_run**: Get full details of a Katalon test run
- **rerun_test_run**: Returns the newly created test run ID.

Re-run an existing Katalon test run
- **list_test_results**: Returns durations, statuses, and error messages.

List detailed test results within a test run
- **get_test_result**: Get full details of a single Katalon test result
- **list_execution_environments**: List execution environments in a Katalon project
- **list_project_releases**: Returns release names, scheduled dates, and aggregated test run statistics.

List defined releases in a Katalon project
- **list_project_builds**: Returns build identifier names, IDs, and the count of associated test runs.

List software builds in a Katalon project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Katalon TestOps (AI Test Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 test runs in project 'E-commerce API' (ID: 123)"

**🤖 AI Agent:**
> I've retrieved the latest 5 test runs for project 123. Highlights: Run #987 (Passed), Run #986 (Failed - 2 errors), Run #985 (Passed). Would you like to inspect the results for the failed run?

---

**👤 You:**
> "Rerun test run ID 986"

**🤖 AI Agent:**
> Rerunning test run 986… New active execution started. New Run ID: 988. I'll let you know once the results are available. Would you like me to notify you if it fails again?

---

**👤 You:**
> "What are the active releases defined in project 123?"

**🤖 AI Agent:**
> I've identified 2 active releases in project 123: 'Q1 Spring Update' (v1.2.0) and 'Hotfix Security' (v1.2.1). Release v1.2.0 has 45 associated test runs with a 98% pass rate. Would you like a detailed build report?


## ❓ FAQ

**Q: Can I rerun a failed test suite using my agent?**
Yes. Use the `rerun_test_run` tool by providing the ID of the failed execution. Your agent will trigger a fresh run using the exact same configuration and return the new Test Run ID for tracking.

**Q: How do I see the screenshots from a specific test failure?**
Ask your agent to `get_test_result` for a specific result ID. If the test was configured to capture visuals, your agent will retrieve the screenshot links along with diagnostic logs and error messages.

**Q: Can I check which browser versions were used in a test run?**
Absolutely. Use the `list_execution_environments` tool for your project. Your agent will return detailed OS, browser, and device configurations used for executions, ensuring you have the full technical context.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/katalon-testops-ai-test-management](https://vinkius.com/mcp/katalon-testops-ai-test-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Katalon TestOps (AI Test Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `katalon-testops-ai-test-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Katalon TestOps (AI Test Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "katalon-testops-ai-test-management": {
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
