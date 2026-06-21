# Clickatell MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickatell)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clickatell-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clickatell-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage mobile messaging via Clickatell — send SMS, track delivery status, monitor balance, and handle inbound rules directly from any AI agent.

## Description
Connect your **Clickatell** account to any AI agent and take full control of your global mobile messaging workflows through natural conversation.

### What you can do

- **SMS Dispatch** — Send single or bulk SMS messages natively with support for E.164 formatting and Unicode payloads
- **Delivery Tracking** — Perform structural extraction of properties driving final carrier statuses to confirm your messages reached cellular towers
- **Account Management** — Monitor your available API balance and check international network coverage for specific numbers
- **Campaign Monitoring** — List scheduled text blasts and audit delivery timings strictly within Clickatell limits
- **Inbound Reply Rules** — Create and manage keyword-based reply rules and webhooks to automate two-way messaging flows

### How it works

1. Subscribe to this server
2. Enter your Clickatell API Key (found in the 'API Integrations' section of your Clickatell Portal)
3. Start managing your mobile communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — monitor scheduled campaigns and check delivery success rates without leaving the workspace
- **Customer Support** — send individual notifications and audit message statuses to resolve delivery inquiries
- **Operations Managers** — track account balances and verify international carrier coverage for global operations
- **Developers** — test and manage inbound reply rules and webhooks through natural conversation


## Available Tools
- **test_carrier_coverage**: Dispatch an automated validation check routing MSISDN routes
- **upsert_inbound_rule**: Bootstrap an entirely empty structural parsing block allocating Webhooks
- **wipe_inbound_rule**: Obliterate mapped HTTP Logic bounds avoiding legacy routing
- **get_account_balance**: Retrieve explicit Cloud metrics tracing active Funding Limits
- **get_delivery_status**: Perform structural extraction of properties driving final Carrier statuses
- **list_scheduled_campaigns**: Identify precise active arrays spanning Marketing boundaries
- **list_inbound_rules**: Enumerate explicitly attached structured rules traversing MO bounds
- **dispatch_bulk_sms**: 164 boundaries optimizing Clickatell pipeline bandwidth directly avoiding API lag.

Identify bounded routing spaces bridging concurrent SMS arrays
- **dispatch_sms_message**: 164 natively.

Provision a massively scalable JSON Payload rendering outbound SMS natively over Clickatell
- **cancel_queued_message**: Irreversibly vaporize explicit SMS blocks deleting scheduled drops


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clickatell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send SMS to +1234567890: 'Your order #987 is ready for pickup!'"

**🤖 AI Agent:**
> Message dispatched! Message ID: msg_abc123. The SMS has been sent to +1234567890 via the Clickatell gateway. I can check the delivery status for you in a few moments.

---

**👤 You:**
> "What is my current Clickatell account balance?"

**🤖 AI Agent:**
> Your current balance is $45.20. Based on your recent activity, this is enough for approximately 2,200 more domestic SMS messages.

---

**👤 You:**
> "Check delivery status for message ID msg_789"

**🤖 AI Agent:**
> Status for msg_789: 'Delivered to Gateway'. The message has successfully passed the Clickatell nodes and has been handed off to the local carrier for final delivery.


## Installation & Usage

To install and use the **Clickatell** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickatell](https://vinkius.com/mcp/clickatell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
