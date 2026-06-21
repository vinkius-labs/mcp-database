# Honeybadger (Error Tracking) MCP Server

Monitor app exceptions and uptime via Honeybadger — list projects, resolve faults, and track deployments.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/honeybadger-error-tracking)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Honeybadger** account to any AI agent and take full control of your exception monitoring and application health through natural conversation.

### What you can do

- **Project Management** — List all monitored projects and extract high-level details including API keys, languages, and unresolved fault counts directly from your agent
- **Fault Analysis** — Query fault groups (error aggregates) to understand class names, messages, and environment distributions across your infrastructure
- **Resolution Workflow** — Mark faults as resolved or ignore them to maintain a clean error dashboard and ensure your team stays focused on critical issues
- **Notice Inspection** — Deep-dive into individual error occurrences (notices) to retrieve backtraces, request data, session context, and server environments
- **Uptime & Deployment** — Monitor site availability and track recent deployment revisions to identify if a specific code change triggered new regressions
- **Team Audit** — List registered team members and their roles to understand notification distribution and ownership for specific projects

### How it works

1. Subscribe to this server
2. Enter your Honeybadger Personal Auth Token
3. Start monitoring your application health from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — debug exceptions and inspect backtraces through natural conversation without leaving your IDE or switching to the browser
- **SREs & DevOps** — monitor global uptime sites and track deployment histories to ensure infrastructure stability and code quality
- **Engineering Leads** — audit unresolved fault counts and team assignments to optimize bug-fixing workflows and incident response


## Available Tools
- **list_projects**: Returns project names, IDs, tokens, language, environments, and fault/notice counts.

List all projects in Honeybadger
- **get_project**: Get full details of a Honeybadger project
- **list_faults**: Returns class names, messages, environments, occurrence counts, and first/last noticed dates.

List faults (error groups) for a Honeybadger project
- **get_fault**: Get full details of a Honeybadger fault
- **resolve_fault**: Irreversible matrix state change.

Resolve a Honeybadger fault
- **list_notices**: List notices (individual error occurrences) for a Honeybadger fault
- **get_notice**: Get full details of a Honeybadger notice
- **list_sites**: List uptime monitoring sites in a Honeybadger project
- **list_members**: List team members on a Honeybadger project
- **list_deployments**: List recent deployments registered in a Honeybadger project


## Installation & Usage

To install and use the **Honeybadger (Error Tracking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/honeybadger-error-tracking](https://vinkius.com/mcp/honeybadger-error-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
