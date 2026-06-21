# Plivo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plivo-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plivo-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plivo-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your Plivo communications — send SMS and audit calls via AI.

## Description
Empower your AI agent to orchestrate your entire cloud communication infrastructure with **Plivo**, the enterprise-grade platform for messaging and voice. By connecting Plivo to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and retrieve call logs without you ever touching a technical console. Whether you are providing customer notifications or managing corporate voice lines, your agent acts as a real-time telecom operator, ensuring your communication is always reliable and your usage data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages instantly and retrieve detailed message status and history.
- **Call Auditing** — List all recent voice calls and retrieve metadata for each, including duration and status.
- **Number Oversight** — List and monitor all phone numbers associated with your account.
- **Pricing Insights** — Retrieve detailed pricing information for messaging and voice services across different countries.
- **Application Governance** — List configured Plivo applications to ensure your communication logic is correctly applied.

### How it works

1. Subscribe to this server
2. Enter your Plivo Auth ID and Auth Token
3. Start managing your cloud communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication usage and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery statuses and audit call logs without manual dashboard logins.
- **Developers** — perform rapid audits of project configurations and test messaging pipelines through natural language.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_account**: Get Plivo account details
- **get_call**: Get details for a specific call
- **get_message**: Get details for a specific message
- **list_applications**: List Plivo applications
- **list_calls**: List recent voice calls
- **list_messages**: List recent SMS messages
- **list_phone_numbers**: List Plivo phone numbers
- **list_pricing**: Get pricing for a country
- **make_call**: Start an outbound call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Plivo phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' and '+44 987 654 321'. Both are active and configured for voice and SMS.

---

**👤 You:**
> "Send SMS 'Your appointment is confirmed' to +15550123."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your confirmation to +15550123 using your Plivo number. The message UUID is xxxxxxxx.

---

**👤 You:**
> "What is the SMS pricing for Brazil?"

**🤖 AI Agent:**
> I've retrieved the pricing for Brazil (BR). Outbound SMS is $0.05 per message, and inbound is free for mobile numbers. Would you like the voice rates as well?


## Installation & Usage

To install and use the **Plivo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plivo-alternative](https://vinkius.com/mcp/plivo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
