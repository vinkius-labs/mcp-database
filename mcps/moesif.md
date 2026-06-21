# Moesif MCP Server

Monitor and analyze API traffic with Moesif — log events, track user/company profiles, and query API analytics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/moesif)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect **Moesif** to your AI agent to gain deep visibility into your API ecosystem. This server allows you to log traffic, manage user/company metadata, and perform complex analytical queries using Elasticsearch DSL without leaving your conversation.

### What you can do

- **Event Logging** — Record single or batch API requests and responses to the Moesif Collector for real-time monitoring.
- **User & Company Tracking** — Upsert profiles with custom metadata (MRR, email, plan type) to link API usage to specific customers.
- **Advanced Analytics** — Search through historical events or count occurrences using powerful Elasticsearch DSL filters.
- **Time-Series Queries** — Filter data by specific time ranges (e.g., last 24 hours, last month) and time zones.

### How it works

1. Subscribe to this server
2. Provide your Moesif Application ID and Management API Key
3. Start debugging and analyzing your API traffic through Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Debug failing API calls and inspect request/response payloads directly from the IDE.
- **Product Managers** — Track feature adoption and API usage trends without building custom dashboards.
- **Customer Success** — Quickly identify which users are experiencing errors or hitting rate limits.


## Available Tools
- **count_events**: Count events matching a filter
- **log_event**: Log a single API call to Moesif
- **log_events_batch**: Log API calls in batch to Moesif
- **search_events**: Use post_filter, size, and sort.

Search events using Elasticsearch DSL
- **update_company**: Upsert a company profile in Moesif
- **update_user**: Upsert a user profile in Moesif


## Installation & Usage

To install and use the **Moesif** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moesif](https://vinkius.com/mcp/moesif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
