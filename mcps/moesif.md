# Moesif MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moesif)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moesif-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moesif-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor and analyze API traffic with Moesif — log events, track user/company profiles, and query API analytics directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moesif** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Count how many API calls resulted in a 401 Unauthorized error in the last 7 days."

**🤖 AI Agent:**
> I've queried Moesif using `count_events`. There were 142 instances of 401 Unauthorized errors between -7d and now.

---

**👤 You:**
> "Update user 'user_123' in Moesif with email 'dev@example.com' and plan 'Enterprise'."

**🤖 AI Agent:**
> I've updated the profile for 'user_123' using `update_user`. The metadata now includes the new email and plan details.

---

**👤 You:**
> "Search for the last 5 API requests made to the '/v1/payments' endpoint."

**🤖 AI Agent:**
> Using `search_events`, I found the 5 most recent requests to '/v1/payments'. Most were successful (200 OK), but one returned a 402 Payment Required. Would you like to see the body of that specific event?


## Installation & Usage

To install and use the **Moesif** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moesif](https://vinkius.com/mcp/moesif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
