# FullStory MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fullstory)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fullstory-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fullstory-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage digital experience intelligence, track users, and retrieve session data via AI agents with FullStory.

## Description
Connect your **FullStory** account to any AI agent to automate your digital experience intelligence (DXI) and product analytics workflows through the Model Context Protocol (MCP). FullStory provides a comprehensive view of how users interact with your site or app. This MCP server enables you to manage user profiles, track server-side events, and retrieve session metadata and playback links directly through natural conversation.

### Key Features

- **User Lifecycle Management** — List all captured users, fetch detailed profile metadata, and upsert records to maintain accurate identity mapping.
- **Session Oversight** — Retrieve a list of recording sessions for specific users and access playback URLs to visualize the customer journey.
- **Interaction Events** — Fetch the complete set of captured events (clicks, navigations, custom events) for any specific session ID.
- **Server-Side Tracking** — Log custom interaction events programmatically from your backend to enrich your FullStory datasets.
- **Segment Discovery** — Access and list configured user segments to understand high-level audience behavior.
- **Data Exports** — Monitor and list generated raw data bundles for deeper analytical processing.
- **Privacy Compliance** — Programmatically delete user data to support GDPR and CCPA requests via simple AI commands.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FullStory API Key (found in Settings > API Keys)
3. Start managing your DXI data from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers & Analysts** — quickly check user activity or find specific session playbacks without manual dashboard navigation.
- **Support Engineers** — get a real-time overview of a customer's recent interaction events while troubleshooting issues.
- **Privacy Officers** — automate the deletion of user records for compliance audits via simple AI commands.


## Available Tools
- **delete_user**: Permanently removes privacy-sensitive telemetry, custom property links, and session aggregations inside FullStory.

Erase a user profile and their associated session history
- **get_account_info**: Validates live integration capability and fetches workspace scope definitions.

Verify authentication and retrieve basic platform stats
- **get_session_events**: Exposes click trails, navigation mutations, error logs, and precise structural DOM changes.

Fetch the chronological telemetry events for a session
- **get_session**: Resolves page transitions, total active time, event markers, and active direct access tracking links.

Retrieve deep metadata for a specific session recording
- **get_user**: Retrieves raw session metadata, total session durations, custom variables, and cross-device interaction boundaries.

Get full tracking profile and behavior history for a specific user
- **list_exports**: Resolves the status of bulk data offloads, processing states, and download URIs for warehouse ingestion.

List raw data export jobs available for download
- **list_segments**: Resolves saved audience definitions, population counts across the last 30 days, and logical filter structures.

List dynamic audience segments built in FullStory
- **list_sessions**: Resolves a subset of sessions matching provided JSON query criteria, exposing playback links, browser signatures, and metric overlays.

List or search session recordings based on telemetry
- **list_users**: Resolves user identities, custom parameters, session counts, and aggregate behavioral profiles across the analytics boundary.

Query the FullStory subscriber and visitor directory for analytics
- **create_event**: Automatically mapped for server-side metrics injection that bypassed the frontal JavaScript client.

Dispatch a custom backend event into FullStory
- **create_update_user**: Used to synchronize custom tenant data into the FullStory analytics boundary for enhanced session context.

Upsert a user identity into FullStory tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FullStory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 sessions for user UID 'user_12345'."

**🤖 AI Agent:**
> Retrieving sessions... I found 5 recent recording sessions for UID user_12345. Key sessions include a 'Checkout' flow from yesterday and a 'Login' event from this morning. Which playback link would you like?

---

**👤 You:**
> "Show me the full profile details for FullStory ID '123:456'."

**🤖 AI Agent:**
> Fetching user data... For ID 123:456, I found email 'customer@example.com'. They are part of the 'Premium' segment and have 15 custom properties, including 'total_spent: 150.00'.

---

**👤 You:**
> "Track a server event 'Subscription Renewed' for user 'johndoe@email.com'."

**🤖 AI Agent:**
> Event tracked! I have successfully posted the 'Subscription Renewed' event to FullStory for johndoe@email.com. This data will now appear in their user timeline.


## Installation & Usage

To install and use the **FullStory** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fullstory](https://vinkius.com/mcp/fullstory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
