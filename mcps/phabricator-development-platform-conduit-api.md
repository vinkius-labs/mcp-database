# Phabricator (Development Platform Conduit API) MCP Server

Manage tasks, code reviews, and repositories via Phabricator's Conduit API — search Maniphest tasks, edit revisions, and query users directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/phabricator-development-platform-conduit-api)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Phabricator** instance to any AI agent to streamline your development workflow. This server leverages the Conduit API to provide deep integration with Maniphest, Differential, and Diffusion.

### What you can do

- **Task Management (Maniphest)** — Search for tasks using complex filters, create new tasks, or update existing ones (status, owners, comments) using `maniphest_search` and `maniphest_edit`.
- **Code Reviews (Differential)** — Query and search for code revisions, or perform actions like accepting and requesting changes via `differential_revision_search` and `differential_revision_edit`.
- **Repository Insights (Diffusion)** — List and filter repositories or search for specific commits using `diffusion_repository_search` and `diffusion_commit_search`.
- **Audit History** — Retrieve the full transaction history of any task to understand its lifecycle with `maniphest_gettasktransactions`.
- **User Management** — Identify the authenticated user or search for other contributors across the platform.

### How it works

1. Subscribe to this server
2. Provide your Phabricator Instance URL and Conduit API Token
3. Start managing your monorepo and tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Software Engineers** — Check task details or update code revisions without leaving your IDE.
- **Release Managers** — Track commit history and repository status across the entire organization.
- **Project Leads** — Audit task histories and manage sprint progress through natural language queries.


## Available Tools
- **differential_query**: Query Differential revisions (Legacy)
- **differential_revision_edit**: Create or update a Differential revision
- **differential_revision_search**: Search for Differential revisions
- **diffusion_commit_search**: Search for Diffusion commits
- **diffusion_repository_search**: Search for Diffusion repositories
- **maniphest_edit**: Create or update a Maniphest task
- **maniphest_gettasktransactions**: Get transaction history for a task
- **maniphest_search**: Supports complex filtering via constraints.

Search for Maniphest tasks
- **user_search**: Search for users
- **user_whoami**: Get details about the authenticated user


## Installation & Usage

To install and use the **Phabricator (Development Platform Conduit API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phabricator-development-platform-conduit-api](https://vinkius.com/mcp/phabricator-development-platform-conduit-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
