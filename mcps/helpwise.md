# Helpwise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpwise)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/helpwise-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/helpwise-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Collaborate on customer emails, SMS, and WhatsApp messages in shared team inboxes with assignment and automation rules.

## Description
Connect your **Helpwise** account to any AI agent and manage your shared inboxes through natural conversation.

### What you can do

- **Mailbox Management** — List all shared mailboxes (email, SMS, WhatsApp, social) with status and configuration
- **Conversation Tracking** — Browse conversations in any mailbox and inspect individual threads with full message history
- **Contact Management** — List all contacts and create new customer profiles with email and name
- **Email Sending** — Send outgoing emails or replies through any connected mailbox
- **Team Overview** — List all agents and team members linked to your account

### How it works

1. Subscribe to this server
2. Enter your Helpwise API Key and API Secret from account settings
3. Start managing your inbox from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Teams** — review conversations, reply to customers, and manage contacts without switching to the Helpwise dashboard
- **Team Leads** — monitor inbox activity, track response times, and oversee team workloads
- **Operations Managers** — audit communication history and manage contact databases through AI


## Available Tools
- **create_contact**: Create a new contact
- **get_conversation_details**: Get details for a specific conversation
- **list_contacts**: List Helpwise contacts
- **list_conversations**: List conversations in a mailbox
- **list_mailboxes**: List Helpwise shared inboxes
- **list_team_members**: List team users
- **send_email**: Send an outgoing email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helpwise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all shared mailboxes and the latest conversations in the support inbox."

**🤖 AI Agent:**
> You have 4 shared mailboxes: 1) 'Support' (mailbox_1, email, 12 open conversations). 2) 'Sales' (mailbox_2, email, 5 open). 3) 'WhatsApp Business' (mailbox_3, WhatsApp, 8 open). 4) 'Info' (mailbox_4, email, 3 open). Latest conversations in 'Support': 1) 'Billing issue — double charge' from john@example.com (2 hours ago, 4 messages). 2) 'API integration help' from dev@techco.com (3 hours ago, 6 messages). 3) 'Password reset request' from sarah@company.com (5 hours ago, 2 messages). Would you like to read a specific conversation or send a reply?

---

**👤 You:**
> "Create a new contact for 'Maria Silva' and send her a welcome email from the support mailbox."

**🤖 AI Agent:**
> Contact created! Name: Maria Silva, Email: maria@example.com, ID: contact_4521. Now sending welcome email via 'Support' mailbox (mailbox_1)... ✅ Email sent! To: maria@example.com, Subject: 'Welcome to Our Support', Body: Professional welcome message with onboarding links. The conversation will appear in the Support inbox once Maria replies. Would you like to list all contacts or send another email?

---

**👤 You:**
> "List all team members and show the full thread for the billing conversation."

**🤖 AI Agent:**
> Team members: 6 agents. 1) Sarah Chen (Admin, online). 2) Mike Torres (Agent, online). 3) Lisa Park (Agent, away). 4) James Rodriguez (Agent, offline). 5) Ana Müller (Agent, online). 6) Bot Agent (Automation). Billing conversation thread (conv_8901, 4 messages): [Customer 2h ago]: 'I was charged twice for my subscription. Order #12345.' [Mike 1h30m ago]: 'I apologize for the inconvenience. Let me check your account.' [Customer 1h ago]: 'Please fix this ASAP, I need the refund.' [Mike 45m ago]: 'I've initiated a refund for the duplicate charge. You should see it within 3-5 business days.' Status: Awaiting customer confirmation. Would you like to send a follow-up or close this conversation?


## Installation & Usage

To install and use the **Helpwise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpwise](https://vinkius.com/mcp/helpwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
