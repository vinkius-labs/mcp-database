# Codecov MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/codecov)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage test coverage and engineering metrics via Codecov — track coverage reports, monitor commit totals, and audit code quality directly from any AI agent.

## Description
Connect your **Codecov** account to any AI agent and take full control of your test coverage and engineering insights through natural conversation. Streamline how you monitor software quality across your repositories natively.

### What you can do

- **Repository Oversight** — List and retrieve details for all repositories including their current coverage percentage natively
- **Commit Intelligence** — Access aggregate coverage totals for specific commit SHAs to verify build health flawlessly
- **Report Hierarchy** — Retrieve a hierarchical view of coverage reports matching your project's file structure flawlessly
- **Branch & Flag Logistics** — Monitor coverage across different branches and custom flags to understand distribution securely
- **Developer Insights** — Access your own user profile and core account metadata directly within your workspace flawlessly
- **integrated Visibility** — Retrieve detailed repository metadata including service provider and owner information flawlessly

### How it works

1. Subscribe to this server
2. Enter your Codecov Global API Token (obtained from Settings > Access)
3. Start managing your test coverage from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — monitor coverage changes and audit specific file reports using natural language
- **Engineering Managers** — review team coverage trends and repository health without opening the dashboard
- **DevOps Engineers** — quickly look up commit coverage totals and verify build status straight from their chat interface
- **Quality Assurance** — verify test completeness and monitor coverage flags across platforms


## Available Tools
- **get_commit_coverage_totals**: Retrieve aggregate coverage totals for a specific commit SHA
- **get_my_codecov_profile**: Retrieve information about the authenticated user
- **get_repository_coverage_details**: Get detailed coverage information for a specific repository
- **get_coverage_report_tree**: Retrieve a hierarchical view of the coverage report matching the file structure
- **list_repository_branches**: List all branches tracked in Codecov
- **list_repository_commits**: List recent commits and their coverage status
- **list_coverage_flags**: List all coverage flags defined for a repository
- **list_codecov_repositories**: List all repositories associated with an owner


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Codecov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all repositories for the organization 'vinkius' on GitHub."

**🤖 AI Agent:**
> Retrieving repositories for gh/vinkius... I found 5 items including 'core-api' (85.4% coverage), 'web-frontend' (92.1% coverage), and 'mcp-connectors' (78.0% coverage). Would you like to see the report tree for any of these?

---

**👤 You:**
> "What is the coverage for the latest commit in 'core-api'?"

**🤖 AI Agent:**
> Checking coverage for the latest commit... SHA 'abc1234' has an overall coverage of 85.4%. It has 1,200 hits, 150 misses, and 50 partials. This matches the target threshold.

---

**👤 You:**
> "Show me the coverage report tree for 'web-frontend'."

**🤖 AI Agent:**
> Retrieving report tree for web-frontend... The project has excellent coverage overall (92.1%). The 'src/components' folder is at 95%, while 'src/utils' is slightly lower at 88%.


## ❓ FAQ

**Q: Can I see the coverage percentage for a specific commit?**
Yes! Use the `get_commit_coverage_totals` tool with the commit SHA. The agent will return the aggregate coverage percentage, hits, misses, and other metrics for that specific version of the code.

**Q: How do I check the coverage distribution across my project's folders?**
Use the `get_coverage_report_tree` tool. Your agent will fetch a hierarchical view of the report, showing you exactly which directories have high coverage and which need more tests.

**Q: Where do I find my Codecov API Token?**
Log in to your Codecov account, go to **Settings**, and select **Access**. You can generate and copy a new API token from the 'Tokens' section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codecov](https://vinkius.com/mcp/codecov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Codecov** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `codecov` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Codecov** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "codecov": {
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
