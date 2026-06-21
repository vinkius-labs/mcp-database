# Cordial MCP Server

Equip your AI agent to manage subscribers, campaigns, and automated messaging through the Cordial Marketing API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cordial)

## Overview
**Category:** communication-messaging
**Tools Count:** 10

## Description
Integrate **Cordial**, the cross-channel marketing platform, directly into your AI workflow. Manage your audience segments, trigger automated messages, and monitor campaign performance using natural language.

### What you can do

- **Audience Management** — List and search for subscribers, and update profile attributes seamlessly.
- **Campaign Monitoring** — Track the performance of batch and transactional email/SMS campaigns.
- **Automation Control** — Monitor and manage active message automation workflows.
- **Data Insights** — Access supplementary data collections and account metadata via chat.

### How it works

1. Connect the Cordial integration to your AI assistant.
2. Authorize using your Cordial API Key.
3. Orchestrate your marketing operations through intuitive conversation.

### Who is this for?

- **CRM Managers** — Quickly update subscriber data or check segment sizes.
- **Email Marketers** — Monitor real-time open and click rates for active campaigns.
- **Marketing Operations** — Audit automation workflows and supplementary data tables.


## Available Tools
- **upsert_subscriber**: Creates or updates a profile with identity properties, channel preferences, and custom attributes.

Create or update a subscriber profile
- **get_account_details**: Resolves system-level account identifiers, plan configuration, and core platform settings.

Get metadata about your Cordial account
- **get_subscriber_profile**: Resolves granular profile data including custom attributes, device tokens, and list memberships.

Get full profile and attributes for a subscriber
- **list_automation_messages**: Resolves active automated message definitions and workflow status for triggered communications.

List active automated message workflows
- **list_marketing_campaigns**: Resolves campaign identity and status, including scheduling data and high-level performance indicators.

List marketing campaigns and their performance
- **list_contacts**: Resolves contact identity properties including email addresses, channel opt-ins, and attribute metadata across the Cordial system boundary.

List subscribers in Cordial
- **list_audience_segments**: Resolves list identity properties such as segment IDs, names, and subscriber counts.

List contact segments and audience groups
- **list_messages**: Resolves batch and transactional message definitions, including templates, subject lines, and sender profiles.

List batch and transactional messages
- **list_supplementary_data**: Resolves metadata for custom data collections used for message personalization.

List supplement collections (external data tables)
- **search_campaigns_by_name**: Resolves a subset of campaigns matching the name criteria across the platform boundary.

Search for marketing campaigns by name


## Installation & Usage

To install and use the **Cordial** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cordial](https://vinkius.com/mcp/cordial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
