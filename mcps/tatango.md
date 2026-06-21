# Tatango MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tatango)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tatango-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tatango-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Run high-volume SMS and MMS campaigns for enterprise marketing with compliance tools that keep you TCPA-safe at scale.

## Description
Connect your **Tatango** account to any AI agent and simplify how you manage your high-volume SMS marketing, subscriber lists, and campaign outreach through natural conversation.

### What you can do

- **Subscriber Management** — List and search subscribers, add new phone numbers to lists, and handle unsubscribes programmatically.
- **Broadcast Campaigns** — Create and send mass SMS campaigns to specific marketing lists and monitor their performance.
- **Transactional SMS** — Send one-to-one non-marketing messages like alerts, receipts, and notifications.
- **List Oversight** — Manage your marketing directories by listing and inspecting metadata for each subscriber list.
- **Webhook Monitoring** — List active webhooks to ensure your outbound events and integrations are running smoothly.
- **Account Visibility** — Fetch your profile details and check API health directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Tatango API Key (found in your account settings)
3. Start managing your SMS outreach from Claude, Cursor, or any MCP client

### Who is this for?

- **Political & Non-Profit Teams** — quickly execute mass alerts and manage large subscriber lists via simple AI commands.
- **Marketing Managers** — monitor campaign statuses and verify list growth directly from the workspace.
- **Operations Leads** — automate transactional notifications and verify API connectivity via the AI assistant.


## Available Tools
- **add_new_sms_subscriber**: Can trigger an opt-in confirmation.

Add a subscriber to a list
- **check_api_health**: Verify Tatango API connectivity
- **create_broadcast_campaign**: Create and send a broadcast message
- **get_list_details**: Get details for a specific list
- **get_account_profile**: Get authenticated account info
- **get_subscriber_details**: Get info for a specific phone number
- **list_sms_campaigns**: List all broadcast campaigns
- **list_sms_marketing_lists**: List all marketing lists
- **list_sms_subscribers**: List subscribers for a specific list
- **list_configured_webhooks**: List active webhooks
- **send_transactional_sms**: g., receipt, alert) to a phone number. Max 160 chars.

Send a one-to-one transactional message
- **unsubscribe_phone_number**: Remove a subscriber from a list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tatango** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my SMS marketing lists."

**🤖 AI Agent:**
> I've retrieved your marketing lists. You have 3 active directories: 'Main Supporters' (1,250 members), 'Event Leads', and 'Volunteer Alerts'. Which one would you like to see subscribers for?

---

**👤 You:**
> "Send a broadcast to the 'Volunteer Alerts' list: 'Meeting relocated to Hall B. See you there!'."

**🤖 AI Agent:**
> Broadcast initiated! I've triggered the campaign to the 'Volunteer Alerts' list (ID: 10293). All subscribers in that group will receive the update shortly.

---

**👤 You:**
> "Add +15550199 to the 'Main Supporters' list."

**🤖 AI Agent:**
> Subscriber added! I've registered +15550199 in the 'Main Supporters' list. They will now receive your upcoming broadcast alerts.


## Installation & Usage

To install and use the **Tatango** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tatango](https://vinkius.com/mcp/tatango)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
