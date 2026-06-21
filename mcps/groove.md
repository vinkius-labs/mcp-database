# Groove MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/groove)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/groove-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/groove-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your customer support tickets via Groove — list conversations, reply to customers, and monitor agent activity directly via AI.

## Description
Connect your **Groove** helpdesk account to any AI agent and take full control of your customer support operations through natural conversation.

### What you can do

- **Ticket Orchestration** — List all support tickets and retrieve specific conversation summaries natively
- **Live Customer Reply** — Draft and send replies or internal notes to specific tickets flawlessy
- **Status Management** — Update ticket states including opened, pending, and closed to keep your inbox organized synchronously
- **Agent Oversight** — List active support agents and retrieve individual productivity details natively
- **Customer Navigation** — Search and retrieve customer profiles, including their full contact history flawlessly
- **Mailbox Coordination** — List and inspect all configured mailboxes to manage multi-channel support synchronously

### How it works

1. Subscribe to this server
2. Enter your Groove API Access Token (found in your Groove Dashboard under Account Settings > API)
3. Start managing your helpdesk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly summarize long ticket threads and audit agent responses via natural language
- **Customer Success Managers** — monitor high-priority tickets and update customer details directly through the chat interface
- **Small Business Owners** — manage customer inquiries and close resolved tickets flawlessly without opening the main dashboard synchronously


## Available Tools
- **create_message**: Add a reply or internal note to a ticket
- **create_ticket**: Create a new helpdesk ticket
- **get_agent**: Get details for a specific agent by email
- **get_customer**: Get details for a specific customer by email
- **get_mailbox**: Get details for a specific mailbox by ID
- **get_ticket**: Get details for a specific ticket by its number
- **list_agents**: List all agents in the Groove account
- **list_customers**: List all customers in the Groove account
- **list_mailboxes**: List all mailboxes in the account
- **list_messages**: List all messages and comments in a ticket
- **list_tickets**: List all helpdesk tickets
- **update_ticket_state**: Change the status of a ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my open tickets in Groove"

**🤖 AI Agent:**
> Retrieving your open tickets... I found 5 tickets requiring attention, including #402: 'Billing Inquiry' and #405: 'Login Issue'. Would you like me to summarize the latest message for the login issue?

---

**👤 You:**
> "Show the messages for ticket #405"

**🤖 AI Agent:**
> Fetching conversation history... Ticket #405 contains 3 messages. The customer reported they cannot reset their password. There is also an internal note from Agent Sarah mentioning a potential database sync delay.

---

**👤 You:**
> "Reply to ticket #402: 'Your refund has been issued and should appear in 3-5 days'"

**🤖 AI Agent:**
> Sending reply... Success! I've posted the message to Ticket #402 informing the customer about their refund. The ticket state remains 'pending'. Should I mark it as closed?


## Installation & Usage

To install and use the **Groove** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/groove](https://vinkius.com/mcp/groove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
