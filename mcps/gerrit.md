# Gerrit MCP Server

Manage code reviews via Gerrit — query changes and patch sets, handle reviewers and approvals, and audit project branches directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gerrit)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Gerrit Code Review** instance to any AI agent and take full control of your collaborative code reviews, project repositories, and patch set management through natural conversation.

### What you can do

- **Change & Review Orchestration** — Query Gerrit changes using advanced syntax like 'status:open' or 'owner:self' to retrieve subjects, numbers, and owners natively
- **Patch Set Auditing** — List all revisions (patch sets) of a change to track commit SHAs, uploader info, and parent commits for detailed version history flawlessly
- **Reviewer & Approval Oversight** — Enumerate reviewers on any change and retrieve approval labels (Code-Review, Verified) to monitor the consensus process synchronousy
- **Project & Repository Navigation** — List all projects and retrieve detailed metadata including states (ACTIVE/READ_ONLY) and default branch configurations securely
- **Branch Management** — Identify and list all branches within a Gerrit project, extracting the latest commit SHAs to verify repository boundaries natively
- **Account & Identity Discovery** — Fetch authenticated user profile information and list associated verified email addresses to verify account contexts flawlessy
- **Group & Access Auditing** — List all Gerrit groups to identify who controls access to projects and grants specific permissions within your organizational tree

### How it works

1. Subscribe to this server
2. Enter your Gerrit URL, Username, and HTTP Password (found in your Gerrit Settings > HTTP Password)
3. Start managing your code reviews from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers & Maintainers** — track open changes and review patch sets without leaving the chat or IDE interface
- **Engineering Managers** — audit code review progress and verify approval labels using natural language conversation
- **DevOps Engineers** — test and debug Gerrit API integrations and verify project branch structures in real-time
- **SRE Teams** — monitor project states and verify organizational group permissions through natural conversation


## Available Tools
- **query_changes**: Uses syntax: "status:open", "owner:self", "project:myproj". Returns subjects, numbers, statuses, owners, projects, patches.

Query changes (code reviews) on Gerrit
- **get_change**: Get full details of a Gerrit change
- **list_projects**: List all projects (repositories) on Gerrit
- **get_project**: Get full details of a Gerrit project
- **list_branches**: List all branches in a Gerrit project
- **get_account**: Get the authenticated Gerrit account
- **list_emails**: List all email addresses associated with the authenticated Gerrit account
- **list_reviewers**: List all reviewers on a Gerrit change
- **list_patchsets**: List all patch sets (revisions) of a Gerrit change
- **list_groups**: Returns group names, IDs, owners, and descriptions.

List all groups on Gerrit


## Installation & Usage

To install and use the **Gerrit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gerrit](https://vinkius.com/mcp/gerrit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
