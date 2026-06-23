# GitHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/github-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage repositories, issues, pull requests and workflows via GitHub — search code, audit commits and track CI/CD from any AI agent.

## Description
Connect your **GitHub** account to any AI agent and take full control of your development workflows through natural conversation.

### What you can do

- **User & Repository Discovery** — View your profile and list all repositories with visibility, language and star counts
- **Issue Management** — List, inspect and create issues with labels and Markdown descriptions
- **Pull Request Tracking** — Browse and review pull requests with merge status, draft state and review info
- **Commit History** — Review commit logs across branches with author, message and timestamp
- **Release Management** — List releases and fetch specific release details by git tag
- **CI/CD Monitoring** — Check recent GitHub Actions workflow runs with status and conclusion
- **Advanced Search** — Search repositories using GitHub's powerful query syntax with language, stars and org qualifiers

### How it works

1. Subscribe to this server
2. Enter your GitHub Personal Access Token
3. Start managing your repos from Claude, Cursor, or any MCP-compatible client

No more context-switching to GitHub.com to check PR status or audit issues. Your AI acts as a dedicated engineering lead.

### Who is this for?

- **Developers** — quickly check issue status, review PRs and inspect commits without leaving your IDE
- **Engineering Managers** — audit open issues, track release progress and monitor CI/CD health across repositories
- **Open Source Maintainers** — review community issues, triage pull requests and manage release tags via conversation


## Available Tools (14)
- **create_issue**: Requires the owner, repo and title. Optionally set the issue body (Markdown text) and labels (comma-separated). Returns the created issue with its number, title and URL.

Create a new GitHub issue
- **get_issue**: Provide the owner, repo and issue number.

Get details for a specific GitHub issue
- **get_user**: Returns login, name, email, avatar URL, company, bio, public repos count, followers and following counts. Use this to verify your token is working correctly.

Get the authenticated GitHub user
- **get_pull_request**: Provide the owner, repo and PR number.

Get details for a specific GitHub pull request
- **get_release_by_tag**: Returns the release name, tag name, body (Markdown), draft/prerelease status, publish date and attached assets. Provide the owner, repo and tag name.

Get a GitHub release by its tag name
- **get_repo**: Provide the owner (org or user) and repo name.

Get details for a specific GitHub repository
- **list_branches**: Each branch includes its name, commit SHA and whether it is the default (protected) branch.

List branches in a GitHub repository
- **list_commits**: Optionally filter by branch (sha parameter) and set the number of results. Each commit includes the SHA, author, commit message and date. Results are ordered newest first.

List commits on a GitHub repository branch
- **list_issues**: Optionally filter by state (open, closed, all). Note: GitHub's issues endpoint includes pull requests — use list_pull_requests for PRs only. Returns issue number, title, state, labels, assignee and creation date.

List issues in a GitHub repository
- **list_pull_requests**: Optionally filter by state (open, closed, all). Returns PR number, title, state, author, draft status, creation date and merge status. Use get_pull_request for full details on a specific PR.

List pull requests in a GitHub repository
- **list_releases**: Each release includes its tag name, name, draft/prerelease status, author, publish date and asset downloads info. Returns the most recent releases first.

List releases for a GitHub repository
- **list_repos**: Optionally filter by type (all, owner, public, private, member) and set the number of results per page. Returns repo name, full_name, description, visibility, language, stars, forks and creation date.

List repositories for the authenticated user
- **list_workflow_runs**: Optionally filter by branch and set the number of results. Each run includes its ID, workflow name, event trigger, status (queued, in_progress, completed), conclusion (success, failure), branch and creation date.

List GitHub Actions workflow runs for a repository
- **search_repos**: The query supports qualifiers like "language:typescript", "stars:>1000", "org:microsoft", "pushed:>2024-01-01" and free-text search. Results include repo name, description, stars, forks, language and creation date.

Search GitHub repositories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all open issues in my backend-api repo."

**🤖 AI Agent:**
> I found 7 open issues in backend-api. The most critical is #142 'Database connection timeout on high load' (bug, high-priority, assigned to @alice). Other notable issues include #138 'Add rate limiting middleware' and #135 'Refactor auth middleware to support OAuth2'.

---

**👤 You:**
> "What's the status of recent workflow runs on main branch?"

**🤖 AI Agent:**
> The last 5 workflow runs on main: CI Pipeline (success, 12m ago), Deploy to Staging (success, 10m ago), Security Scan (success, 8m ago), Release Build (failure, 2h ago — failed at 'build Docker image' step) and Integration Tests (success, 3h ago).

---

**👤 You:**
> "Search for popular Python machine learning repos with over 1000 stars."

**🤖 AI Agent:**
> I found several highly-starred Python ML repos: huggingface/transformers (119k stars), scikit-learn/scikit-learn (58k stars), tensorflow/tensorflow (185k stars), pytorch/pytorch (79k stars) and microsoft/ML-For-Beginners (27k stars). Would you like more details on any of these?


## ❓ FAQ

**Q: How do I create a GitHub Personal Access Token?**
Go to [**Settings > Developer settings > Personal access tokens**](https://github.com/settings/tokens), click **Generate new token (classic)**, give it a descriptive name, select the scopes you need (recommended: repo, workflow, read:org) and click **Generate token**. Copy the token immediately — it starts with `ghp_` and won't be shown again.

**Q: Can I create issues with labels via the agent?**
Yes! Use the `create_issue` tool with the owner, repo and title parameters. Optionally provide a Markdown body and comma-separated labels (e.g. "bug,high-priority"). The agent will create the issue and return its number, title and URL.

**Q: How do I search for repositories with specific criteria?**
Use the `search_repos` tool with GitHub's query syntax. Examples: "machine learning in:name language:python stars:>1000" finds Python ML repos with 1k+ stars; "org:microsoft pushed:>2024-01-01" finds Microsoft repos updated in 2024. The query supports qualifiers for language, stars, forks, org, topic, size and more.

**Q: Does this tool support GitHub Actions workflow monitoring?**
Yes! Use `list_workflow_runs` to see recent CI/CD executions for a repository. You can filter by branch and see each run's status (queued, in_progress, completed) and conclusion (success, failure, cancelled). This is useful for checking if recent deployments or builds passed without opening the Actions tab.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github-alternative](https://vinkius.com/mcp/github-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `github-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "github-alternative": {
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
