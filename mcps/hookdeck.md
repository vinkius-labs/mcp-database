# Hookdeck MCP Server

Manage and monitor webhooks with Hookdeck — list connections, create sources, and control event routing directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hookdeck)

## Overview
**Category:** developer-tools
**Tools Count:** 52

## Description
Connect your **Hookdeck** account to any AI agent to orchestrate your webhook infrastructure through natural conversation. Hookdeck provides the reliability layer for your event-driven architecture, and this server puts that power in your chat interface.

### What you can do

- **Connection Management** — List, create, and update connections that route webhooks from sources to destinations.
- **Traffic Control** — Instantly pause or resume event routing for specific connections to manage maintenance windows or outages.
- **Source Monitoring** — Retrieve and count your webhook sources to understand where your incoming data originates.
- **Lifecycle Operations** — Enable or disable connections and manage their rules via JSON payloads without leaving your workflow.
- **Deep Inspection** — Fetch specific metadata for any connection or source using unique IDs to debug routing issues.

### How it works

1. Subscribe to this server
2. Enter your Hookdeck API Key
3. Start managing your webhook reliability layer from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Engineers** — quickly toggle webhook traffic or check connection statuses during deployments.
- **DevOps Teams** — monitor the health of event-driven pipelines and manage sources programmatically.
- **Integration Specialists** — verify routing rules and connection counts across different environments.


## Available Tools
- **cancel_event**: Cancel scheduled retries for an event
- **count_connections**: Count total connections
- **count_sources**: Count total sources
- **create_bookmark**: Create a new bookmark
- **create_connection**: Create a connection
- **create_destination**: Create a new destination
- **create_issue_trigger**: Create a new issue trigger
- **create_source**: Create a new source
- **create_transformation**: Create a new transformation
- **delete_bookmark**: Remove a bookmark
- **delete_connection**: Permanently delete a connection
- **delete_destination**: Delete a destination
- **delete_issue_trigger**: Delete an issue trigger
- **delete_source**: Delete a source
- **disable_connection**: Disable a connection
- **disable_source**: Disable a source
- **enable_connection**: Enable a disabled connection
- **enable_source**: Enable a source
- **get_attempt**: Retrieve a specific attempt
- **get_connection**: Retrieve a specific connection
- **get_destination**: Retrieve a specific destination
- **get_event**: Retrieve a specific event
- **get_issue_trigger**: Retrieve a specific issue trigger
- **get_metrics_attempts**: Delivery attempt metrics
- **get_metrics_events**: Event processing statistics
- **get_metrics_queue_depth**: Current queue depth per destination
- **get_metrics_requests**: Request volume metrics
- **get_metrics_transformations**: Transformation execution performance
- **get_request**: Retrieve a specific request
- **get_source**: Retrieve a specific source
- **get_transformation**: Retrieve a specific transformation
- **list_attempts**: Retrieve a list of delivery attempts
- **list_bookmarks**: Retrieve a list of bookmarks
- **list_connections**: Retrieve a list of connections
- **list_destinations**: Retrieve a list of destinations
- **list_events**: Retrieve a list of events
- **list_issue_triggers**: Retrieve a list of issue triggers
- **list_requests**: Retrieve a list of requests
- **list_sources**: Retrieve a list of sources
- **list_transformations**: Retrieve a list of transformations
- **pause_connection**: Pause event routing for a connection
- **retry_event**: Manually retry a failed event
- **retry_request**: Retry a rejected request
- **test_transformation**: Test transformation code against a payload
- **trigger_bookmark**: Replay the bookmarked request
- **unpause_connection**: Resume event routing for a connection
- **update_connection**: Update a connection rules or name
- **update_destination**: Update destination config (URL, rate limit, etc.)
- **update_issue_trigger**: Update an issue trigger
- **update_source**: Update a source
- **update_transformation**: Update transformation code
- **upsert_connection**: Create or update a connection by name


## Installation & Usage

To install and use the **Hookdeck** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hookdeck](https://vinkius.com/mcp/hookdeck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
