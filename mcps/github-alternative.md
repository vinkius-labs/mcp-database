# GitHub MCP Server

Manage repositories, issues, pull requests and workflows via GitHub — search code, audit commits and track CI/CD from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/github-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 14

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


## Installation & Usage

To install and use the **GitHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github-alternative](https://vinkius.com/mcp/github-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
