# GitLab MCP Server

Manage projects, track issues, and oversee CI/CD pipelines via AI agents with GitLab.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gitlab)

## Overview
**Category:** industry-titans
**Tools Count:** 16

## Description
Connect your **GitLab** instance to any AI agent to automate your DevSecOps lifecycle and project management through the Model Context Protocol (MCP). GitLab is the most comprehensive AI-powered platform for software innovation. This MCP server enables you to retrieve project metadata, manage issues, track merge requests, and monitor CI/CD pipelines directly through natural conversation.

### Key Features

- **Project Oversight** — List all accessible projects, fetch detailed configuration metadata, and track forks across your instance.
- **Issue & MR Management** — List issues and merge requests, track their lifecycle status, and programmatically open new issues from your chat interface.
- **CI/CD Visibility** — Retrieve a list of pipelines for any project to monitor build and deployment health in real-time.
- **Repository Discovery** — Access the contents of files within any repository to understand codebase structures and documentation.
- **Global Search** — Execute powerful searches across projects, issues, and users to isolate specific development artifacts.
- **Identity Oversight** — Access detailed profile information for the authenticated user to verify permissions and account context.
- **Real-time Synchronization** — Keep your development and operations data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GitLab Base URL and Personal Access Token (found in User Settings)
3. Start managing your projects from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Tech Leads** — quickly check the status of a merge request or list open issues without manual dashboard navigation.
- **Project Managers** — get a real-time overview of pipeline health and project activity via simple AI commands.
- **DevOps Engineers** — automate the retrieval of file contents and project metadata for auditing and automation.


## Available Tools
- **verify_api_connection**: Check connection
- **create_project_issue**: Open an issue
- **get_repository_file**: Read file content
- **get_my_gitlab_profile**: Get user identity
- **create_merge_request**: Requires title.

Create a new merge request
- **get_merge_request**: Use the IID (the MR number shown in the UI, not the internal ID).

Get details for a specific merge request
- **list_branches**: List all branches in a project repository
- **list_project_members**: List all members of a project
- **get_project_details**: Get project metadata
- **list_visible_groups**: List accessible groups
- **list_project_issues**: List project issues
- **list_merge_requests**: List merge requests
- **list_project_pipelines**: List CI/CD pipelines
- **list_project_forks**: List forks
- **list_visible_projects**: List accessible projects
- **search_gitlab_global**: Search all GitLab


## Installation & Usage

To install and use the **GitLab** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitlab](https://vinkius.com/mcp/gitlab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
