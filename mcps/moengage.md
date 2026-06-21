# MoEngage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moengage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moengage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moengage-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Engage mobile app users with personalized push notifications, in-app messages, and AI-optimized customer journeys across channels.

## Description
Connect your **MoEngage** account to any AI agent and manage customer engagement through natural conversation.

### What you can do

- **User Management** — Create/update user attributes and device data
- **Event Tracking** — Track custom user events and behaviors
- **Push Notifications** — Trigger transactional and marketing push messages
- **Campaign Management** — Launch and pause multi-channel campaigns
- **Analytics** — Retrieve campaign performance and user statistics

### How it works

1. Subscribe to this server
2. Enter your MoEngage Workspace ID and API Key
3. Start managing customer engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — orchestrate omnichannel campaigns
- **Product Teams** — track user behavior and engagement
- **Developers** — integrate server-side events and push notifications


## Available Tools
- **check_moengage_status**: Verify connectivity
- **get_campaign_stats**: Get campaign stats
- **get_campaign**: Get campaign details
- **get_customer**: Get customer details
- **get_segment**: Get segment details
- **list_campaigns**: List campaigns
- **list_segments**: List segments
- **search_customers**: Search customers
- **send_push**: Send push notification
- **track_events_bulk**: Track events in bulk
- **track_event**: Track an event
- **update_device**: Update device info
- **upsert_customer**: Create or update customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoEngage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show performance for the 'Spring Sale Push' campaign."

**🤖 AI Agent:**
> Campaign Analytics: 'Spring Sale Push'. Sent: 145,000. Delivered: 142,500 (98%). Clicks: 12,400 (8.7% CTR ⭐). Conversions: 3,200 Purchases ($45K revenue). Uninstalls attributed: 12.

---

**👤 You:**
> "Send a transactional push notification to user 8901."

**🤖 AI Agent:**
> Push notification sent! ✅ Target: User_8901. Title: 'Order Shipped 📦'. Message: 'Your order #1234 is on the way!'. Platform: iOS. Status: Success (Delivered to 1 device).

---

**👤 You:**
> "Track a 'Subscription Upgraded' event for user Sarah."

**🤖 AI Agent:**
> Event tracked! ✅ User ID: sarah@company.com. Event: 'Subscription Upgraded'. Properties: {plan: 'Pro', amount: 45.00, platform: 'Web'}. Profile updated successfully.


## Installation & Usage

To install and use the **MoEngage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moengage](https://vinkius.com/mcp/moengage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
