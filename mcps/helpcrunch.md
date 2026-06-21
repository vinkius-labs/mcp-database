# HelpCrunch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpcrunch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/helpcrunch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/helpcrunch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer support via HelpCrunch — manage chats, customers, and team assignments directly from any AI agent.

## Description
Connect your **HelpCrunch** account to any AI agent and take full control of your customer communication and support workflows through natural conversation.

### What you can do

- **Chat Oversight** — List all active and past conversations, retrieve full transcripts, and monitor response times.
- **Customer Management** — Access detailed customer profiles, add descriptive tags, and track user interaction history.
- **Team Coordination** — Reassign chats to specific team members or departments to ensure the right person handles every query.
- **Proactive Support** — Search through chats using complex filters to identify trends or urgent customer issues.
- **Workflow Automation** — Update chat statuses (closed, open, snoozed) directly from the chat interface.
- **Operational Efficiency** — List support departments and monitor the overall health of your customer service operations.

### How it works

1. Subscribe to this server
2. Enter your HelpCrunch API Key (found in Settings > Developers)
3. Start managing your customer support from Claude, Cursor, or any MCP-compatible client

No more jumping between multiple dashboard tabs. Your AI assistant acts as a dedicated Support Lead or Customer Success Manager.

### Who is this for?

- **Support Managers** — instantly retrieve chat summaries and check team workloads without digging through reports.
- **Customer Success Teams** — check client history and add updates or tags during follow-ups.
- **Sales Development Reps** — monitor new inbound chats and qualify leads directly from the communication flow.


## Available Tools
- **add_customer_tag**: Add a label/tag to a customer profile
- **send_message**: Pass the payload as a JSON string in "body_json" (e.g., {"chat": 123, "text": "Hello"}).

Send a message to a chat
- **get_chat_details**: Get detailed information about a specific chat
- **get_customer_details**: Get detailed profile information for a specific customer
- **list_chats**: Each chat includes basic metadata and status.

List all conversations (chats) in HelpCrunch
- **list_customers**: List all customers (contacts) in HelpCrunch
- **list_departments**: List all support departments
- **list_chat_messages**: Useful for understanding context or historical interactions.

List all messages within a specific chat
- **search_chats**: Pass filter criteria as a JSON string in "filter_json" (e.g., {"status": "open"}).

Search for chats using filters
- **update_chat_assignee**: Assign a chat to a specific team member
- **update_chat_status**: Update the status of a chat (e.g., closed, open)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HelpCrunch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open chats and show the last message for each."

**🤖 AI Agent:**
> I've retrieved your open chats. You have 3 active conversations: 'Billing query' from Sarah, 'API Issue' from Mark, and 'Feedback' from Elena. Sarah's last message was 'When is my next invoice?'. Would you like to see the full transcript for any of these?

---

**👤 You:**
> "Search for all chats from the customer with email 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching database... I found 2 historical chats for John Doe. The first was about 'Onboarding' (Closed) and the second is an 'Upgrade Request' (Pending). Should I retrieve the messages for the pending request?

---

**👤 You:**
> "Tag customer ID 5592 with 'VIP' and 'Priority Support'."

**🤖 AI Agent:**
> Tags added! I've successfully applied the 'VIP' and 'Priority Support' labels to customer 5592. They will now be clearly identified in your dashboard. Should I also check if they have any open chats?


## Installation & Usage

To install and use the **HelpCrunch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpcrunch](https://vinkius.com/mcp/helpcrunch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
