# Vonage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vonage-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vonage-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vonage-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage your Vonage communications — send SMS and audit account data via AI.

## Description
Empower your AI agent to orchestrate your entire cloud communication infrastructure with **Vonage** (formerly Nexmo), the flexible platform for messaging and voice. By connecting Vonage to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and check your account balance without you ever touching a technical dashboard. Whether you are providing secure notifications or managing global communication profiles, your agent acts as a real-time telecom operator, ensuring your connection is always reliable and your data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages instantly and retrieve detailed message status and account balance.
- **Account Auditing** — List all phone numbers associated with your profile and retrieve detailed metadata for each.
- **Pricing Insights** — Query real-time pricing for messaging and voice services across different countries.
- **Inventory Discovery** — Search for available phone numbers by country and type to expand your reach.
- **Community Management** — List users and conversations to maintain a structured view of your communication channels.

### How it works

1. Subscribe to this server
2. Enter your Vonage API Key and API Secret
3. Start managing your cloud communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication spend and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery and audit conversation threads without manual dashboard logins.
- **Developers** — perform rapid audits of application configurations and test messaging pipelines through natural language.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_balance**: Get Vonage account balance
- **get_pricing**: Get pricing for a country
- **list_account_secrets**: List account secrets
- **list_applications**: List Vonage applications
- **list_conversations**: List recent conversations
- **list_phone_numbers**: List Vonage phone numbers
- **list_search_numbers**: Search for available phone numbers
- **list_users**: List Vonage users
- **list_voice_calls**: List recent voice calls
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vonage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Vonage phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '1234567890' and '0987654321'. Both are currently active and ready for use.

---

**👤 You:**
> "Check my Vonage account balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have €15.42 available in your account. I can also check the pricing for your next message if you like.

---

**👤 You:**
> "Search for available mobile numbers in the UK."

**🤖 AI Agent:**
> I've found 5 available mobile numbers in the UK (GB). Examples include '447700900123' and '447700900456'. Would you like the full metadata for any of them?


## Installation & Usage

To install and use the **Vonage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vonage-alternative](https://vinkius.com/mcp/vonage-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
