# GitHub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/github-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/github-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/github-alternative-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **GitHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github-alternative](https://vinkius.com/mcp/github-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
