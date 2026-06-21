# TestMonitor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/testmonitor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

List QA projects, extract test runs, read user assignments, and fetch tracked issues strictly from your AI chat.

## Description
Link up your **TestMonitor** cloud infrastructure with any AI agent to streamline QA tracking operations and retrieve real-time milestone data without having to navigate web dashboards.

### What you can do

- **Project Triage** — List all ongoing projects alongside their high-level metadata such as test coverage and delivery status
- **Runs & Milestones Tracking** — Instantly retrieve project-scoped test runs, milestones lists, and deadline progress
- **Defect Auditing** — Query all generated issues or software defects explicitly linked to a specific test project
- **Requirement Tracing** — Ask the agent to map requirements against existing feature specifications without manually matching them in the UI
- **Team Management Lookup** — Easily list out all the users provisioned in the workspace to confirm roles or debugging ownership

### How it works

1. Subscribe to this server
2. Provide your Subdomain and your Personal Access Token
3. Coordinate your entire QA suite from Claude, Cursor, or any compatible AI IDE

### Who is this for?

- **Quality Directors** — request a quick summary of the current Test Runs and their respective Milestones before daily stand-ups
- **Bug Triagers** — leverage the AI to list reported defects and quickly assign the contextual backlog data to new tickets
- **Product Owners** — read the explicit specifications of any Requirement and cross-reference against active test cases without breaking focus


## Available Tools (10)
- **get_test_case_details**: Retrieves full details for a specific TestMonitor test case
- **get_project_details**: Retrieves details for a specific TestMonitor project
- **get_test_run_details**: Retrieves details for a specific TestMonitor test run
- **list_test_cases**: Lists all test cases within a specific TestMonitor project
- **list_issues**: Lists all issues (defects) within a project
- **list_milestones**: Lists all milestones within a project
- **list_projects**: Project IDs are required for most other tools.

Lists all projects available on the TestMonitor instance
- **list_requirements**: Lists all requirements for a project
- **list_test_runs**: Lists all test runs within a specific project
- **list_account_users**: Lists all users associated with the TestMonitor account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TestMonitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all TestMonitor projects."

**🤖 AI Agent:**
> Found 1 project:
`ID: 8840` | Name: "Vinkius CRM Engine V2" | Status: **Active**
I can retrieve the related milestones, test cases, or registered issues matching ID 8840.

---

**👤 You:**
> "Get me the details for Test Case ID 5521 from project 8840."

**🤖 AI Agent:**
> Detailing Case `5521` (API Logout Auth Rejection):
- **Status:** Approved
- **Requirement ID Linked:** REQ-10
- **Step 1:** Force invalid Bearer string to the `/auth/logout` endpoint. Expected: Returns raw 401 HTTP unauthorized block immediately.
- **Step 2:** Ensure cache header remains un-poisoned. Expected: True.
Anything I can rewrite from this?

---

**👤 You:**
> "List all issues for Project 8840."

**🤖 AI Agent:**
> Gathering active issues for Project 8840:
1. **Issue ID:** `ISS-91` | Title: 'Registration Webhook drops payload' | State: In Progress
2. **Issue ID:** `ISS-99` | Title: 'Avatar uploads broken on edge' | State: Open
The project seems to currently host 2 vital reported defects. Should I inspect linked tests for `ISS-91`?


## ❓ FAQ

**Q: Does this tool automate actual user interface tests on websites?**
No. TestMonitor is essentially a Test Management Hub. You document your cases, requirements, runs, and defect reports structurally. The MCP server reads this deep structural data allowing the AI to help correlate bugs to requirements and plan sprints—it does not inherently control a web-browser headless tester to run things.

**Q: Which ID should I pass to fetch Test Runs or Cases?**
Almost all context actions downstream require a `project_id`. Start by telling your prompt: 'List all my TestMonitor projects'. Take the numeric ID corresponding to your target platform, then use it as the anchor for subsequent 'list test cases', 'list runs', or 'list issues' queries.

**Q: Where do I track the Personal Access Token setting?**
It is tied to your individual profile. Log in via web, go to the top right avatar, pick 'My Account', open the 'API' sub-tab, and hit 'Create Token'. Copy it precisely because it is obscured upon closing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testmonitor](https://vinkius.com/mcp/testmonitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TestMonitor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `testmonitor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TestMonitor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "testmonitor": {
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
