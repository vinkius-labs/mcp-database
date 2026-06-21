# CommPeak MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commpeak)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commpeak-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commpeak-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Enable your AI agent to manage dialer campaigns, leads, and send SMS messages via the CommPeak API.

## Description
Connect your AI assistant to **CommPeak**, the cloud communication platform with a powerful dialer and SMS gateway.

### What you can do

- **SMS Messaging** — Send SMS messages to any number using a custom sender ID directly from chat.
- **Campaign Management** — List active dialer campaigns, view their statuses, and manage call queues.
- **Lead Management** — Add new leads to dialer campaigns with phone numbers and contact details.

### How it works

1. Add the CommPeak integration to your AI toolset.
2. Provide your SMS API Token and/or Dialer credentials.
3. Manage your communications via natural language commands.

### Who is this for?

- **Sales Teams** — Add leads to campaigns and trigger SMS outreach without leaving the chat.
- **Call Center Managers** — Monitor campaign statuses and queue metrics in real time.
- **Marketing Teams** — Send targeted SMS messages and track delivery via conversational commands.


## Available Tools
- **create_lead**: Add a new lead to a campaign
- **delete_lead**: Permanently remove a lead from the system
- **get_campaign_details**: Retrieve detailed information about a specific campaign
- **get_lead_details**: Retrieve detailed information about a specific lead
- **get_sms_status**: Retrieve the status of a previously sent SMS
- **list_dialer_campaigns**: Retrieve a list of all dialer campaigns
- **list_leads**: Retrieve leads from a specific campaign
- **list_recent_sms**: Retrieve a list of recently sent SMS messages
- **send_sms**: Send a text message via CommPeak SMS API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CommPeak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to '+1234567890' saying 'Your order has been shipped!'"

**🤖 AI Agent:**
> SMS sent successfully to +1234567890. Message ID: msg-7x2k9. Status: delivered. Sender ID: default.

---

**👤 You:**
> "Show me all active dialer campaigns."

**🤖 AI Agent:**
> You have 3 active campaigns:
1. 'Q1 Outreach' — 450 leads, 62% contacted
2. 'Renewal Follow-up' — 180 leads, 35% contacted
3. 'New Prospects' — 920 leads, 12% contacted
Would you like to add leads to any of these?

---

**👤 You:**
> "Check the delivery status of SMS message ID 'msg-7x2k9'."

**🤖 AI Agent:**
> Message ID 'msg-7x2k9' to +1234567890 was successfully delivered on Oct 25 at 14:30 UTC.


## Installation & Usage

To install and use the **CommPeak** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commpeak](https://vinkius.com/mcp/commpeak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
