# Kissmetrics MCP Server

Track user behavior, set properties, and query analytics data via the Kissmetrics API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kissmetrics)

## Overview
**Category:** marketing-automation
**Tools Count:** 7

## Description
Connect your **Kissmetrics** account to any AI agent to automate your user behavioral analytics and tracking workflows. This MCP server enables your agent to record events, manage user properties, and query complex metric data directly from natural language interfaces.

### What you can do

- **Behavior Tracking** — Record custom events for specific users to monitor their journey and interactions
- **Profile Management** — Set and update user properties and metadata to maintain rich customer profiles
- **Identity Resolution** — Alias multiple identities to maintain a single, unified view of a user across sessions
- **Data Discovery** — List all defined event types and property names currently in your account
- **Analytical Querying** — Retrieve people counts and metric values over time to track business performance

### How it works

1. Subscribe to this server
2. Enter your Kissmetrics API Key
3. Start managing your behavioral data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — Monitor feature adoption and user engagement trends via natural language commands
- **Growth Marketers** — Quickly track campaign conversions and segment user behaviors without writing code
- **Developers** — Integrate server-side event tracking and data retrieval into your development workflow


## Available Tools
- **alias_identities**: g., linking a browser ID to an email).

Link two identities together
- **list_event_types**: List all event types defined in the account
- **list_property_names**: List all property names used in the account
- **query_metric_data**: Requires a metric ID and query parameters.

Get data for a specific metric
- **query_people_count**: Get the count of people matching specific criteria
- **record_event**: Requires a person identity (email/ID) and an event name.

Record a behavior event for a person
- **set_person_properties**: Set properties for a specific person


## Installation & Usage

To install and use the **Kissmetrics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kissmetrics](https://vinkius.com/mcp/kissmetrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
