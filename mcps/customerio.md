# Customer.io MCP Server

Equip your AI agent to manage customer engagement, trigger automated campaigns, and track messaging metrics via the Customer.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/customerio)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

## Description
Integrate **Customer.io**, the platform for sending personalized messages based on customer behavior, directly into your AI workflow. Manage your customer profiles, monitor automated campaigns, and track engagement metrics using natural language.

### What you can do

- **Customer Identification** — Create or update customer profiles with behavioral attributes via the Identify API.
- **Campaign Monitoring** — List automated campaigns and retrieve real-time performance and engagement metrics.
- **Broadcast & Newsletter Tracking** — Track one-to-many broadcast messages and newsletter statuses.
- **Segment Oversight** — Explore dynamic and manual customer segments to understand your audience composition.

### How it works

1. Connect the Customer.io integration to your AI assistant.
2. Authorize using your Customer.io Site ID and API Key (found in Settings > API Keys).
3. Orchestrate your customer engagement strategy through intuitive conversation.

### Who is this for?

- **Retention Marketers** — Quickly audit campaign performance and customer segment sizes.
- **Growth Engineers** — Identify and update customer profiles with behavioral data via chat.
- **Support Teams** — Retrieve full customer profiles and messaging history to provide personalized assistance.


## Available Tools
- **identify_customer**: Resolves the identification status and profile state. Mutates the workspace identity database.

Create or update a customer profile with attributes
- **get_campaign_performance**: Resolves sent, opened, clicked, and converted counts. Interacts with the analytics and reporting engine.

Get delivery and engagement metrics for a campaign
- **get_engagement_summary**: Resolves high-level engagement KPIs. Interacts with the global analytics boundary.

Retrieve a high-level summary of campaign and broadcast performance
- **get_customer_details**: Resolves custom attributes, device tokens, and segment memberships. Touches the granular profile and behavioral data boundary.

Get full profile, attributes, and devices for a specific customer
- **list_broadcast_messages**: Resolves broadcast identifiers and scheduling metadata. Interacts with the bulk messaging boundary.

List all one-to-many broadcast messages
- **list_automated_campaigns**: Resolves campaign IDs, names, and trigger types. Interacts with the automation and messaging boundary.

List all automated messaging campaigns
- **list_newsletters**: Resolves newsletter IDs and status. Touches the content distribution and newsletter management boundary.

List all newsletter campaigns
- **list_customers**: Resolves unique identifiers, email addresses, and last-seen timestamps. Interacts with the core identity and profile boundary.

List all customers/people in your Customer.io workspace
- **list_customer_segments**: Resolves segment IDs, types (manual/dynamic), and membership counts. Touches the audience segmentation and filtering boundary.

List all dynamic and manual segments
- **search_customers_by_email**: Resolves the associated customer identifiers. Touches the identity lookup and search boundary.

Search for a customer profile by email address


## Installation & Usage

To install and use the **Customer.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customerio](https://vinkius.com/mcp/customerio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
