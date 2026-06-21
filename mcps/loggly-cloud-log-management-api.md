# Loggly (Cloud Log Management API) MCP Server

Manage cloud logs via Loggly — send events, execute Lucene searches, and analyze infrastructure metrics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/loggly-cloud-log-management-api)

## Overview
**Category:** devops-cicd
**Tools Count:** 8

## Description
Connect your **Loggly** account to any AI agent to streamline your observability and debugging workflows. This MCP server allows you to interact with your logs using natural language, making it easier to find errors, monitor performance, and manage your logging infrastructure.

### What you can do

- **Log Ingestion** — Send single or bulk log events (plaintext or JSON) directly to Loggly for real-time indexing.
- **Advanced Search** — Execute complex queries using Lucene syntax to filter through millions of events across specific timeframes.
- **Result Retrieval** — Fetch paginated search results using Result Set IDs (rsid) for deep analysis of system behavior.
- **Field Analysis & Faceting** — List available log fields and get value counts (faceting) to understand data distribution and common errors.
- **Account Management** — Retrieve customer info, subscription limits, and list active users and roles within your Loggly organization.

### How it works

1. Subscribe to this server
2. Provide your Loggly Subdomain, API Token, and Customer Token
3. Start querying and sending logs from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to correlate logs. Your AI can now act as a proactive SRE or DevOps engineer, identifying patterns and troubleshooting issues in seconds.

### Who is this for?

- **DevOps & SREs** — Quickly search for production errors and analyze log trends without leaving the terminal or chat interface.
- **Backend Developers** — Send debug events during development and verify log ingestion in real-time.
- **Security Analysts** — Audit user roles and search for suspicious patterns using structured log queries.


## Available Tools
- **get_customer_info**: Retrieve Loggly account details
- **get_events**: Max 5,000 events per search.

Retrieve events for a given search rsid
- **get_field_values**: Get counts of values for a specific field (Faceting)
- **list_fields**: List available fields in Loggly
- **list_users**: Retrieve a list of active users
- **search_events**: Use get_events with the rsid to fetch the actual logs.

Initiate an asynchronous search query
- **send_bulk_events**: The events_data must be line-separated (up to 5MB per batch).

Send batches of line-separated events to Loggly
- **send_event**: Use is_json=true if event_data is a JSON string. Max size 1MB.

Send a single or multiline event to Loggly


## Installation & Usage

To install and use the **Loggly (Cloud Log Management API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loggly-cloud-log-management-api](https://vinkius.com/mcp/loggly-cloud-log-management-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
