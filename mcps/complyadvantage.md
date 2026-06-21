# ComplyAdvantage MCP Server

Automate AML and KYC compliance — screen entities, manage search history, and monitor risks directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/complyadvantage)

## Overview
**Category:** security-compliance
**Tools Count:** 14

## Description
Connect your **ComplyAdvantage** account to any AI agent to streamline your Anti-Money Laundering (AML) and Know Your Customer (KYC) workflows through natural conversation.

### What you can do

- **Entity Screening** — Create new searches for individuals or companies using `create_search` with customizable fuzziness and filters.
- **Search Management** — Retrieve detailed results with `get_search_details` or list previous search history using `list_searches`.
- **Risk Monitoring** — Start or stop ongoing monitoring for specific entities using `update_search_monitors` to stay updated on risk profile changes.
- **Case Collaboration** — Add internal notes with `create_comment` and update search statuses or assignees using `update_search`.
- **Whitelisting & Risk Levels** — Refine entity details and risk classifications directly through the `update_search_entities` tool.

### How it works

1. Subscribe to this server
2. Enter your ComplyAdvantage API Key
3. Start screening and managing compliance risks from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — instantly screen new clients and manage alerts without switching between multiple dashboards.
- **Fintech Developers** — test and verify screening logic directly from the code editor or terminal.
- **Risk & Legal Teams** — automate the gathering of search details and audit trails for regulatory reporting.


## Available Tools
- **acknowledge_monitor**: Acknowledge changes to a monitored search
- **create_comment**: Create a comment on a search or entity
- **create_search**: ) with optional fuzziness and filters.

Create a new search
- **delete_search_tag**: Detach tags from a search
- **get_search_details**: Get full search results
- **get_search_monitors**: Get monitored search details
- **get_search**: Get an overview of a search
- **list_comments**: Retrieve comments for a specific search
- **list_searches**: Get a list of previous searches
- **update_search_entities**: Update entity details (whitelist, risk level)
- **update_search_monitors**: g., start or stop).

Start/stop monitoring
- **update_search_profile**: Update the Search Profile for a monitored search
- **update_search**: Update search details (assignee, status)
- **list_users**: Get a list of users in your account


## Installation & Usage

To install and use the **ComplyAdvantage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/complyadvantage](https://vinkius.com/mcp/complyadvantage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
