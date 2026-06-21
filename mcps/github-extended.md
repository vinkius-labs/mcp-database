# GitHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/github-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage repositories, pull requests, issues, and CI/CD workflows on the world largest developer collaboration platform.

## Description
Connect your **GitHub** account to any AI agent and take full control of your source control and development workflows through natural conversation.

### What you can do

- **Repository Orchestration** — List and manage your repositories programmatically, including retrieving star counts, languages, and detailed metadata
- **Issue Lifecycle** — Monitor project status by listing open issues and creating new ones directly through your agent to maintain momentum
- **Code Intelligence** — Search through repositories and files programmatically to find specific logic and retrieve raw file contents (base64) for analysis
- **Collaboration Visibility** — Monitor pull requests and recent notifications to stay updated on team-wide development activity and code reviews
- **Resource Management** — Access user profiles, organization memberships, and Gists to manage your complete GitHub presence programmatically

### How it works

1. Subscribe to this server
2. Retrieve your **Personal Access Token (PAT)** from GitHub (Settings > Developer Settings > PAT)
3. Ensure your token has the required scopes (repo, user, notifications)
4. Start managing your code and projects from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to check issue statuses. Your AI acts as your dedicated engineering coordinator.

### Who is this for?

- **Software Engineers** — instantly find code snippets across repositories and retrieve file contents using natural language
- **Team Leads** — monitor repository activity and triage issues without leaving your communication tools
- **DevOps Engineers** — automate repository discovery and monitor project notifications through simple AI queries


## Available Tools (12)
- **create_new_issue**: Open GitHub issue
- **get_file_content**: Read file from repo
- **get_my_profile**: Get account info
- **get_repository_details**: Get repo info
- **list_repo_branches**: Check repo branches
- **list_my_gists**: List code snippets
- **list_repository_issues**: List repo issues
- **list_recent_notifications**: Check GitHub inbox
- **list_my_organizations**: List user orgs
- **list_pull_requests**: List repo PRs
- **list_my_repositories**: List your GitHub repos
- **search_repositories**: Find GitHub projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my GitHub repositories and show their stars count."

**🤖 AI Agent:**
> I've retrieved your repositories. You have 12 repos, including 'mcp-server' (150 stars) and 'react-template' (42 stars). Would you like the full metadata for any of these?

---

**👤 You:**
> "Find all open issues in the repository 'vinkius/mcp-server'."

**🤖 AI Agent:**
> Scanning issues for vinkius/mcp-server... I found 3 open issues. Notable ones include 'Fix auth timeout' (ID: 101) and 'Update documentation' (ID: 102). Shall I provide the full description for the auth issue?

---

**👤 You:**
> "Get the content of 'README.md' from repository 'vinkius/mcp-server'."

**🤖 AI Agent:**
> File retrieved! I've fetched the README.md content. It describes the server architecture and installation steps. Would you like me to summarize the main components or explain the setup guide?


## ❓ FAQ

**Q: Can I read private repositories?**
Yes, provided your Personal Access Token (PAT) has the 'repo' scope or appropriate fine-grained permissions for those repositories.

**Q: How do I find a repository owner and name?**
In a GitHub URL like `github.com/vinkius/mcp-server`, the owner is `vinkius` and the repository name is `mcp-server`.

**Q: Does it support creating pull requests?**
This version supports listing pull requests and issues. PR creation is currently handled through the web interface or other specialized tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github-extended](https://vinkius.com/mcp/github-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `github-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "github-extended": {
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
