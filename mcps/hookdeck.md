# Hookdeck MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hookdeck)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and monitor webhooks with Hookdeck — list connections, create sources, and control event routing directly from your AI agent.

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


## Available Tools (52)
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
- **cancel_event**: Cancel scheduled retries for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hookdeck** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Hookdeck connections."

**🤖 AI Agent:**
> I've retrieved your connections. You have 3 active routes: 'Shopify-to-Lambda' (ID: conn_123), 'Stripe-to-Analytics' (ID: conn_456), and 'GitHub-Webhooks' (ID: conn_789).

---

**👤 You:**
> "Pause the connection with ID conn_456 immediately."

**🤖 AI Agent:**
> The connection 'Stripe-to-Analytics' (conn_456) has been successfully paused. Event routing is now suspended.

---

**👤 You:**
> "How many webhook sources do I have?"

**🤖 AI Agent:**
> You currently have a total of 5 sources configured in your Hookdeck project.


## ❓ FAQ

**Q: How can I temporarily stop webhooks from being delivered to a destination?**
You can use the `pause_connection` tool with the specific Connection ID. This will halt event routing until you call `unpause_connection`.

**Q: Can I see how many active sources I have configured?**
Yes, use the `count_sources` tool to get the total number of sources, or `list_sources` to see the details of each one.

**Q: Is it possible to update connection rules through the AI?**
Absolutely. Use the `update_connection` tool by providing the Connection ID and a JSON body containing the new configuration rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hookdeck](https://vinkius.com/mcp/hookdeck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hookdeck** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hookdeck` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hookdeck** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hookdeck": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
