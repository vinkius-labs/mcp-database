# ThoughtSpot MCP Server

Search and analyze business data by interacting directly with your ThoughtSpot metadata and Liveboards via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/thoughtspot)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect your **ThoughtSpot** instance to any AI agent and bring your analytics workflows directly into your chat. Search through your metadata, access reports, and list configurations natively.

### What you can do

- **Metadata Search** — Search for specific analytical assets across your organization and filter by type (Liveboards, Answers, Logical Tables)
- **Browse Visualizations** — List all available Liveboards (dashboards) and Answers (individual charts/tables) without leaving your environment
- **Team Management** — Retrieve lists of registered account users and user groups, along with their access levels
- **Backend Topologies** — List all configured data source connections (such as Snowflake and BigQuery) serving your platform
- **Organization** — Navigate through metadata tags used for classifying data objects and reports

### How it works

1. Subscribe to this server
2. Enter your ThoughtSpot Cloud Host URL, Username, and Secret Key
3. Begin asking your AI agent about your business intelligence infrastructure natively

### Who is this for?

- **Data Engineers** — Verify which backend database connections are currently active without checking the UI
- **Analytics Managers** — Look up available Liveboards, tags, and data views quickly
- **IT Admins** — Interrogate the user directory and group distributions directly from the command line or chat


## Available Tools
- **search_metadata**: Supported types include LIVEBOARD, ANSWER, LOGICAL_TABLE, etc.

Search for metadata objects in ThoughtSpot by type
- **list_liveboards**: Lists all available Liveboards (dashboards)
- **list_answers**: Lists all saved Answers (individual charts or tables)
- **list_account_users**: Lists all users in the ThoughtSpot instance
- **list_user_groups**: Lists all user groups
- **list_data_connections**: g., Snowflake, BigQuery) are connected.

Lists configured data source connections
- **list_metadata_tags**: Lists all tags used for classifying metadata objects


## Installation & Usage

To install and use the **ThoughtSpot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thoughtspot](https://vinkius.com/mcp/thoughtspot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
