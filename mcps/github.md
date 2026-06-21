# GitHub MCP Server

Manage repositories, track issues, and search code via AI agents with GitHub.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/github)

## Overview
**Category:** industry-titans
**Tools Count:** 18

## Description
Connect your **GitHub** account to any AI agent to automate your software development lifecycle and code management through the Model Context Protocol (MCP). GitHub is the world's leading AI-powered developer platform. This MCP server enables you to retrieve repository metadata, manage issues, track pull requests, and search for code directly through natural conversation.

### Key Features

- **Repository Oversight** — List all repositories for any user or organization, and fetch detailed configuration metadata for specific projects.
- **Issue & PR Management** — List issues and pull requests, track their lifecycle status, and programmatically open new issues from your chat interface.
- **Code Content Discovery** — Retrieve the contents of files or directories within any repository to understand codebase structures.
- **Advanced Code Search** — Execute powerful searches across GitHub's massive database to isolate specific code snippets or repositories.
- **Collaboration Tracking** — Monitor forks and contributors to understand project community engagement.
- **Identity Oversight** — Access detailed profile information for the authenticated GitHub user to verify permissions and account context.
- **Real-time Synchronization** — Keep your source control and development data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GitHub Personal Access Token (found in Settings > Developer settings)
3. Start managing your repositories from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Tech Leads** — quickly check the status of a pull request or list open issues without manual dashboard navigation.
- **Project Managers** — get a real-time overview of repository activity and community engagement via simple AI commands.
- **DevOps Engineers** — automate the retrieval of file contents and repository metadata for auditing and workflows.


## Available Tools
- **verify_api_connection**: Check connection
- **list_user_repositories**: List user repos
- **create_pull_request**: Requires the head branch (your changes) and base branch (merge target).

Create a pull request
- **add_issue_comment**: Supports markdown formatting.

Add a comment to an issue or PR
- **create_new_issue**: Open an issue
- **get_file_contents**: Read file content
- **get_issue_details**: Get a specific issue by number
- **get_my_github_profile**: Get user identity
- **get_repository_details**: Get repo metadata
- **list_branches**: List repository branches
- **list_commits**: Optionally filter by branch name or SHA.

List recent commits
- **list_repo_issues**: List repo issues
- **list_org_repositories**: List organization repositories
- **list_pull_requests**: List pull requests
- **list_releases**: List repository releases
- **list_stargazers**: Useful for popularity tracking.

List repository stargazers
- **search_github_code**: Search code snippets
- **search_github_repositories**: Search all repos


## Installation & Usage

To install and use the **GitHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/github](https://vinkius.com/mcp/github)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
