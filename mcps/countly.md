# Countly MCP Server

Manage product analytics via Countly — track user sessions, record custom events, and query deep behavioral metrics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/countly)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect your **Countly** analytics instance to any AI agent to monitor user behavior and application performance through natural conversation.

### What you can do

- **Session Management** — Start, update, and end user sessions to track engagement duration and active users in real-time.
- **Event Tracking** — Record specific user actions with custom keys, counts, and segmentation data to understand feature usage.
- **User Profiling** — Update user details including names, emails, and custom properties to build comprehensive user journeys.
- **Analytics Querying** — Retrieve aggregated metrics for sessions, users, and countries, or fetch detailed data for specific event keys.
- **Advanced Segmentation** — Utilize the Drill API (Enterprise Edition) to perform complex filtering and deep-dive analysis into your data.

### How it works

1. Subscribe to this server
2. Provide your Countly Server URL and API credentials (App Key, API Key, App ID)
3. Start querying your product data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor KPIs and feature adoption rates without navigating complex dashboards.
- **Data Analysts** — perform quick segmentations and event audits using natural language queries.
- **Growth Teams** — track conversion events and user profile updates to optimize marketing funnels.


## Available Tools
- **begin_session**: Starts a new session for a user
- **end_session**: Ends the current session
- **read_drill**: Perform advanced segmentation and filtering (Enterprise Edition)
- **read_events**: Retrieve data for specific custom events
- **read_metrics**: Retrieve standard metrics like sessions, users, or countries
- **record_events**: Records specific actions within the app
- **update_session**: Extends an existing session
- **update_user_details**: Updates information about a specific user


## Installation & Usage

To install and use the **Countly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/countly](https://vinkius.com/mcp/countly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
