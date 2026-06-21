# ActiveTrail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/activetrail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/activetrail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/activetrail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Email and SMS marketing automation — manage contacts, campaigns, and group segments via AI.

## Description
Connect your **ActiveTrail** account to your AI agent to unlock professional email and SMS marketing capabilities. From creating detailed contact profiles to monitoring campaign performance and managing group segments, your agent handles your marketing ecosystem through natural conversation.

### What you can do

- **Contact Management** — Create, update, and list contacts to maintain a healthy and engaged subscriber base
- **Campaign Monitoring** — List active and past email or SMS campaigns and retrieve real-time performance statistics
- **Group Segmentation** — Manage contact groups and segments to ensure your messages reach the right audience
- **SMS Automation** — Send and track SMS messages directly from your chat interface for immediate customer outreach
- **Real-time Analytics** — Quickly audit opens, clicks, and engagement patterns for your marketing efforts

### How it works

1. Subscribe to this server
2. Enter your ActiveTrail API Token
3. Start managing your email and SMS marketing through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — automate campaign audits and list management effortlessly
- **Sales & Growth Teams** — quickly add leads to specific groups and trigger SMS notifications
- **Marketing Operations** — monitor account health and subscriber engagement patterns
- **Small Business Owners** — manage their entire digital marketing presence using simple commands


## Available Tools
- **list_contacts**: Retrieve the full directory of subscribers from the ActiveTrail account
- **create_contact**: Email is required.

Add a new subscriber to the ActiveTrail system with email and personal details
- **list_campaigns**: Retrieve a list of sent and draft email or SMS campaigns in ActiveTrail
- **list_groups**: Retrieve the list of segments and groups configured in the ActiveTrail account
- **send_sms**: Requires the phone number and SMS body text.

Send an immediate SMS text message notification via the ActiveTrail gateway


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ActiveTrail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the performance of my last email campaign."

**🤖 AI Agent:**
> I've retrieved the stats for your 'Summer Sale' campaign. It reached 5,000 subscribers with an open rate of 22% and 450 total clicks. Would you like to see the bounce report?


## Installation & Usage

To install and use the **ActiveTrail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/activetrail](https://vinkius.com/mcp/activetrail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
