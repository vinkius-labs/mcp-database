# Qase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qase)
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


## Available Tools (10)
- **list_plans**: Lists all test plans in a project
- **list_projects**: Lists all projects in Qase
- **list_cases**: Lists test cases in a project
- **get_project**: Retrieves details for a specific project
- **get_case**: Retrieves details for a specific test case
- **list_suites**: Lists test suites in a project
- **list_runs**: Lists all test runs in a project
- **get_run**: Retrieves details for a specific test run
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


## ❓ FAQ

**Q: How do I securely obtain my Qase Token?**
Log in to Qase.io and click your profile icon to go to **Account settings**. Select **API Tokens** (or sometimes found under Apps for an integration token), and click **Create a new API token**. Add a name, click generate, and copy the string provided. It takes exactly 15 seconds. Paste it here to authenticate. Your token is encrypted at rest and injected securely at runtime.

**Q: Can my AI write test scripts using the case details?**
Absolutely. Inside your IDE (like Cursor), you can ask the agent to 'Fetch case #12 from Qase project PROJ'. The tool retrieves the precise steps, preconditions, and expected results. The agent can then automatically generate Playwright, Cypress, or Selenium scripts based exactly on those Qase definitions.

**Q: How can I check the results of a recent QA cycle?**
Ask your agent to `list_runs` for your project. This will surface your recent executions. If you notice a run with a high failure rate, ask the agent to pull `get_run` with that run's ID to dive into specifics and see which modules failed the automated checks.

**Q: Can it help me track Jira bugs linked to tests?**
Yes. By using the `list_defects` capability, your AI can pull all registered defects in a Qase project. If your Qase is integrated with Jira or GitHub, the returned defect data includes external issue links, helping developers immediately map a failed test to the corresponding engineering ticket.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qase](https://vinkius.com/mcp/qase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qase": {
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
