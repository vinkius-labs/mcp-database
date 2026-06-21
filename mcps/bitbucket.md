# Bitbucket MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitbucket)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bitbucket-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bitbucket-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage your Git repositories via Bitbucket — list pull requests, commits, and pipelines directly from any AI agent.

## Description
Connect your **Bitbucket Cloud** account to any AI agent and orchestrate your software development workflows through natural conversation.

### What you can do

- **Repository Oversight** — List all repositories within your workspaces and retrieve detailed metadata.
- **Pull Request Management** — Query and inspect pull requests to monitor code reviews and merge statuses.
- **Commit & Branch Discovery** — List the latest commits and active branches across your projects.
- **CI/CD Monitoring** — Retrieve the status of Bitbucket Pipelines to ensure successful builds.
- **Issue Tracking** — List and retrieve issues for repositories with enabled trackers.
- **Workspace Coordination** — Access and manage your team's workspaces and user profiles.

### How it works

1. Subscribe to this server
2. Enter your Bitbucket Username and App Password
3. Start managing your code from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — quickly check PR statuses and pipeline health without switching tabs.
- **DevOps Engineers** — monitor build statuses and repository activity straight from their workflow tools.
- **Team Leads** — retrieve summaries of recent commits and open issues for daily standups.


## Available Tools
- **get_pull_request**: Get details of a specific pull request
- **list_commits**: List commits for a repository
- **get_repository**: Get details of a specific repository
- **get_user_profile**: Get authenticated user profile
- **list_branches**: List branches for a repository
- **list_issues**: List issues for a repository (if tracker is enabled)
- **list_pipelines**: List CI/CD pipelines for a repository
- **list_pull_requests**: List pull requests for a repository
- **list_repositories**: List repositories in a workspace
- **list_workspaces**: List all accessible workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitbucket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pull requests in repository 'my-app' within workspace 'my-team'."

**🤖 AI Agent:**
> I've retrieved the pull requests for 'my-app'. There are 2 open PRs: 'Feature: New Auth' (ID: 12) and 'Fix: Memory Leak' (ID: 15).

---

**👤 You:**
> "Check the status of the last pipeline run for 'my-app'."

**🤖 AI Agent:**
> The latest pipeline for 'my-app' (Build #452) completed successfully in 3 minutes and 12 seconds.

---

**👤 You:**
> "List the last 5 commits in repository 'my-app'."

**🤖 AI Agent:**
> Retrieving commits... The last 5 commits include updates to the README, a bugfix for the API client, and new tests for the auth module.


## Installation & Usage

To install and use the **Bitbucket** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitbucket](https://vinkius.com/mcp/bitbucket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
