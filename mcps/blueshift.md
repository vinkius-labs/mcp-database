# Blueshift MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blueshift)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blueshift-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blueshift-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Orchestrate customer engagement via Blueshift — manage campaigns, track events, and sync customer data directly from any AI agent.

## Description
Connect your **Blueshift** account to any AI agent and orchestrate your omnichannel marketing and customer data workflows through natural conversation.

### What you can do

- **Campaign Management** — List all marketing campaigns, retrieve detailed execution reports, and monitor high-level performance.
- **Customer Data Orchestration** — Retrieve and update detailed customer profiles, including custom attributes and identifiers.
- **Real-time Event Tracking** — Track custom user interactions (purchases, clicks, views) and retrieve event histories for behavior analysis.
- **Catalog & Segment Discovery** — List all data catalogs and customer segments to ensure accurate targeting.
- **Triggered Campaigns** — Initiate API-triggered campaigns for specific users directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Blueshift User API Key and Site ID
3. Start managing your customer engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Operations** — quickly check campaign statuses and customer profiles without manual dashboard searches.
- **CRM Specialists** — monitor real-time event tracking and customer attributes straight from their workflow tools.
- **Growth Engineers** — verify API integrations and campaign triggers using natural language.


## Available Tools
- **create_update_customer**: Create or update a customer profile
- **get_campaign_detail**: Get detailed report for a specific campaign
- **get_campaign_performance**: Get high-level performance summary for all campaigns
- **get_catalog_items**: Retrieve items from a specific catalog
- **get_customer**: Retrieve a customer profile
- **get_event_history**: Get history of events for a user
- **list_campaigns**: List all marketing campaigns
- **list_catalogs**: List all data catalogs
- **list_segments**: List all customer segments
- **track_event**: Track a custom user event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blueshift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in Blueshift."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Welcome Series V2', 'Summer Re-engagement', and 'Cart Abandonment'.

---

**👤 You:**
> "Show the profile for customer john@example.com."

**🤖 AI Agent:**
> I found the profile for John Doe. Key attributes include: Member since 2023, Total spent $450, and 5 active segments including 'High Value Customers'.

---

**👤 You:**
> "Track a 'purchase' event for user customer_123."

**🤖 AI Agent:**
> Successfully tracked the 'purchase' event for customer_123. The data has been synced to Blueshift and will be reflected in their activity timeline.


## Installation & Usage

To install and use the **Blueshift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blueshift](https://vinkius.com/mcp/blueshift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
