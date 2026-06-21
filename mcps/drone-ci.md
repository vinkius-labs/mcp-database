# Drone CI MCP Server

Automate your CI/CD workflows with Drone CI—manage repositories, monitor builds, and handle secrets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/drone-ci)

## Overview
**Category:** ship-it
**Tools Count:** 39

## Description
Connect your **Drone CI** server to any AI agent to streamline your DevOps lifecycle through natural language.

### What you can do

- **Build Management** — List, get details, restart, or stop builds across your repositories using `list_builds`, `get_build`, and `restart_build`.
- **Repository Control** — Enable, update, or repair repository settings and sync them with your source control provider via `enable_repo` and `sync_user_repos`.
- **Secret & Config Management** — Manage environment secrets, cron jobs, and templates without leaving your chat interface using `list_secrets` and `create_cron_job`.
- **User Administration** — (Admin only) Create, update, or delete users and manage organizational access with `list_users` and `create_user`.
- **Log Inspection** — Fetch build logs to debug pipeline failures instantly using `get_build_logs`.

### How it works

1. Subscribe to this server
2. Provide your Drone Server URL and Personal Access Token
3. Start orchestrating your pipelines from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Monitor pipeline health and trigger builds via voice or text.
- **Software Developers** — Check build logs and status directly from the IDE.
- **SREs** — Manage secrets and cron jobs across multiple projects efficiently.


## Available Tools
- **approve_build**: Approve a blocked build
- **chown_repo**: Change repository ownership to current user
- **create_build**: Create a custom build for a branch
- **create_cron_job**: Create a new cron job
- **create_secret**: Create a new repository secret
- **create_template**: Create a new template
- **create_user**: Create a new user account (Admin)
- **decline_build**: Decline a blocked build
- **delete_cron_job**: Delete a cron job
- **delete_secret**: Delete a repository secret
- **delete_template**: Delete a template
- **delete_user**: Delete a user account (Admin)
- **disable_repo**: Disable or delete a repository
- **enable_repo**: Enable/register a repository in Drone
- **get_build_logs**: Get logs for a specific step in a build stage
- **get_build**: Get specific build info including stages and steps
- **get_cron_job**: Get cron job details
- **get_current_user_repos**: Get current user repositories
- **get_current_user**: Get current authenticated user info
- **get_repo**: Get repository info
- **get_secret**: Get repository secret details
- **get_template**: Get template details
- **get_user**: Get user info by login (Admin)
- **list_builds**: List recent builds for a repository
- **list_cron_jobs**: List cron jobs for a repository
- **list_secrets**: List repository secrets
- **list_templates**: List organization templates
- **list_users**: Requires administrative privileges.

List all registered users (Admin)
- **promote_build**: Promote a build to a target environment
- **repair_repo**: Repair repository webhooks
- **restart_build**: Restart a specific build
- **stop_build**: Stop a running build (Admin)
- **sync_user_repos**: Synchronize user repositories
- **trigger_cron_job**: Manually trigger an existing cron task
- **update_cron_job**: Update a cron job
- **update_repo**: Update repository configuration
- **update_secret**: Update a repository secret
- **update_template**: Update a template
- **update_user**: Update a user account (Admin)


## Installation & Usage

To install and use the **Drone CI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drone-ci](https://vinkius.com/mcp/drone-ci)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
