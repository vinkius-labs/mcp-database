# Code Climate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/code-climate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage code quality and engineering metrics via Code Climate — track repository grades, monitor snapshots, and audit test coverage directly from any AI agent.

## Description
Connect your **Code Climate** account to any AI agent and take full control of your automated code reviews and engineering intelligence through natural conversation. Streamline how you monitor maintainability and test coverage across your repositories natively.

### What you can do

- **Repository Oversight** — List and retrieve details for all repositories analyzed in Code Climate, including health status natively
- **Snapshot Intelligence** — Access current and historical analysis snapshots to understand how code quality evolves flawlessly
- **Issue Management** — List all code issues identified in a specific snapshot to prioritize technical debt securely
- **Coverage Tracking** — Access and monitor test coverage reports to ensure high-quality software delivery flawlessly
- **Webhook Logistics** — Monitor configured webhooks for real-time quality and analysis notifications flawlessly
- **Account Visibility** — Retrieve information about your authenticated user profile and organizational metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Code Climate Personal API Token (found in User Settings)
3. Start managing your code quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Managers** — monitor repository grades and maintainability trends using natural language
- **DevOps Engineers** — audit repository webhooks and analysis status without opening the dashboard
- **Software Developers** — quickly look up specific code issues and test coverage percentages straight from their chat interface
- **Security Teams** — verify repository compliance and monitor static analysis findings


## Available Tools (8)
- **get_my_codeclimate_profile**: Retrieve information about the authenticated user
- **get_repository_code_quality**: Get detailed quality information for a specific repository
- **get_snapshot_quality_details**: Get detailed information for a specific analysis snapshot
- **list_snapshot_code_issues**: List all code issues identified in a specific snapshot
- **list_codeclimate_repositories**: List all repositories analyzed in Code Climate
- **list_repository_snapshots**: List all analysis snapshots for a specific repository
- **list_repository_test_reports**: List all test coverage reports for a repository
- **list_codeclimate_webhooks**: List all configured webhooks for a specific repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Code Climate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my repositories in Code Climate."

**🤖 AI Agent:**
> Retrieving your repositories... I found 5 analyzed projects: 'core-api' (Grade: A), 'frontend-app' (Grade: B), 'mcp-connectors' (Grade: A), and 2 others. Which one would you like to see snapshots for?

---

**👤 You:**
> "What is the current test coverage for the 'core-api' repository?"

**🤖 AI Agent:**
> Checking test coverage for core-api... The most recent report shows 85.4% coverage. This is a 2% increase compared to the previous analysis.

---

**👤 You:**
> "Show me the last 5 analysis snapshots for 'frontend-app'."

**🤖 AI Agent:**
> Retrieving snapshots for frontend-app... I found 5 recent snapshots. The latest was triggered by commit 'abc1234' yesterday, with a maintainability rating of 'B' and 12 issues identified.


## ❓ FAQ

**Q: Can I see the maintainability rating for a specific repository?**
Yes! Use the `get_repository_code_quality` tool with the unique repository ID. The agent will return the current maintainability grade (A-F) and other core health metrics provided by Code Climate.

**Q: How do I check the test coverage percentage for a repository?**
Use the `list_repository_test_reports` tool. Your agent will fetch all test coverage reports associated with the repository, showing the coverage percentage for the most recent runs.

**Q: Where do I find my Code Climate API Token?**
Log in to Code Climate, click on your avatar in the top right, go to **User Settings**, and select **Personal API Tokens**. You can generate and copy your token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/code-climate](https://vinkius.com/mcp/code-climate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Code Climate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `code-climate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Code Climate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "code-climate": {
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
