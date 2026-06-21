# SignalWire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signalwire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/signalwire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/signalwire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your cloud communications — send messages and audit calls via AI.

## Description
Empower your AI agent to orchestrate your entire cloud communication infrastructure with **SignalWire**, the advanced platform for messaging, voice, and video. By connecting SignalWire to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and retrieve call logs without you ever touching a technical console. Whether you are providing customer alerts or managing corporate voice lines, your agent acts as a real-time telecom operator, ensuring your communication is always reliable and your usage data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages instantly and retrieve detailed message status and history.
- **Call Auditing** — List all recent voice calls and retrieve metadata for each, including direction and duration.
- **Number Oversight** — List and monitor all incoming phone numbers associated with your project.
- **Usage Intelligence** — Retrieve detailed usage records to maintain strict organizational control over your communication costs.
- **Account Governance** — Monitor account-wide metadata to understand your project status in real-time.

### How it works

1. Subscribe to this server
2. Enter your SignalWire Project ID, API Token, and Space URL
3. Start managing your cloud communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication usage and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery statuses and audit call logs without manual dashboard logins.
- **Developers** — perform rapid audits of project configurations and test messaging pipelines through natural language.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_account_info**: Get SignalWire account details
- **get_call**: Get details for a specific call
- **get_message**: Get details for a specific message
- **list_calls**: List recent voice calls
- **list_messages**: List recent SMS/MMS messages
- **list_phone_numbers**: List SignalWire phone numbers
- **list_usage**: Get account usage records
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SignalWire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my SignalWire phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' and '+1 987 654 321'. Both are currently active and configured for voice and SMS.

---

**👤 You:**
> "Send SMS 'Server alert: high usage detected' to +15550123."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your alert to +15550123 using your SignalWire number. The message SID is SMxxxx.

---

**👤 You:**
> "Show me recent call logs for my project."

**🤖 AI Agent:**
> I've found 5 recent calls. Notable interactions include an inbound call from '+1 111 2222' lasting 2 minutes. Would you like the full metadata for any specific call?


## Installation & Usage

To install and use the **SignalWire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signalwire](https://vinkius.com/mcp/signalwire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
