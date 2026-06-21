# Kissmetrics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kissmetrics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kissmetrics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kissmetrics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track user behavior, set properties, and query analytics data via the Kissmetrics API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kissmetrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a 'Purchased' event for 'user@example.com' with price 49.99."

**🤖 AI Agent:**
> I've recorded the 'Purchased' event for user@example.com. The price of 49.99 has been successfully attached as a property to this event in Kissmetrics.

---

**👤 You:**
> "Set the property 'Plan Tier' to 'Enterprise' for 'customer_123'."

**🤖 AI Agent:**
> Successfully updated properties for customer_123. The 'Plan Tier' is now set to 'Enterprise' in their behavioral profile.

---

**👤 You:**
> "Show me all event types defined in my account."

**🤖 AI Agent:**
> I've retrieved 15 event types from your Kissmetrics account, including 'Signed Up', 'Logged In', 'Purchased', and 'Feature Used'. Would you like to query metrics for any of them?


## Installation & Usage

To install and use the **Kissmetrics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kissmetrics](https://vinkius.com/mcp/kissmetrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
