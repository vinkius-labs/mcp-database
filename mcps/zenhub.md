# ZenHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage agile boards, epics, and estimates via the ZenHub API.

## Description
Connect your **ZenHub** account to any AI agent to streamline your agile project management on GitHub. This MCP server enables your agent to interact with pipelines, issues, estimates, and epics directly from natural language.

### What you can do

- **Board Visibility** — List all pipelines and issues for specific GitHub repositories or ZenHub workspaces
- **Agile Status Management** — Move issues between pipelines to update their workflow status instantly
- **Precision Estimating** — Set and retrieve story point estimates for any GitHub issue
- **Epic Oversight** — List and inspect ZenHub epics and their constituent issues
- **Release Tracking** — Access release reports and progress metadata for your projects

### How it works

1. Subscribe to this server
2. Enter your ZenHub API Token
3. Start managing your agile workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — Quickly update issue status and estimates from your IDE
- **Project Managers** — Monitor board health and epic progress via natural language commands
- **Scrum Masters** — Facilitate planning by querying release reports and team velocity metrics


## Available Tools
- **get_repo_board**: Get the ZenHub board for a repository
- **get_epic_data**: Get details for a specific epic
- **list_repo_epics**: List all ZenHub epics for a repository
- **set_issue_estimate**: Set the story point estimate for an issue
- **get_zenhub_issue_data**: Get ZenHub-specific metadata for a GitHub issue
- **move_issue_between_pipelines**: Move an issue to a different pipeline
- **list_release_reports**: List release reports for a repository
- **get_workspace_board**: Get the ZenHub board for a specific workspace and repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZenHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the ZenHub board for repository ID '12345678'."

**🤖 AI Agent:**
> I've retrieved the ZenHub board for repository 12345678. You have 5 pipelines: 'New Issues', 'Backlog', 'In Progress', 'Review/QA', and 'Done'. Would you like to see the issues in a specific pipeline?

---

**👤 You:**
> "Move issue #45 in repo '12345678' to the 'In Progress' pipeline (ID: '56789') in workspace '98765'."

**🤖 AI Agent:**
> Successfully moved issue #45 to the 'In Progress' pipeline in your ZenHub workspace.

---

**👤 You:**
> "What are the estimates for all issues in the current epic?"

**🤖 AI Agent:**
> For the current epic, I found 8 issues. Total estimated points: 34. Current distribution: 3 issues (8 pts), 2 issues (5 pts), 3 issues (3 pts).


## ❓ FAQ

**Q: How do I find my GitHub Repository ID?**
You can find your Repository ID in your GitHub settings, or use a GitHub MCP server to query your repository metadata.

**Q: Can I move an issue to a different pipeline using this agent?**
Yes, the `move_issue_between_pipelines` tool allows you to specify a workspace, repository, issue number, and target pipeline ID to update the status.

**Q: Is it possible to set story point estimates?**
Absolutely. Use the `set_issue_estimate` tool with the repository ID, issue number, and your desired point value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenhub](https://vinkius.com/mcp/zenhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZenHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zenhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZenHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenhub": {
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
