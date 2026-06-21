# Gorgias MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gorgias)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gorgias-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gorgias-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your customer support tickets, messages, and user profiles via AI.

## Description
Connect your **Gorgias** helpdesk to your AI agent and streamline your customer support operations. Use natural language to monitor ticket queues, draft replies, and manage customer profiles without switching tabs.

### What you can do

- **Ticket Management** — List open tickets, retrieve specific conversation histories, and update ticket statuses
- **Customer Communication** — Draft and send replies to customers or add internal notes for your team
- **Customer Profiles** — Search for customers by email, retrieve their details, or create new profiles on the fly
- **Team Monitoring** — List active agents and retrieve user details for internal coordination

### How it works

1. Subscribe to this server
2. Enter your Gorgias Subdomain, Email, and REST API Key
3. Start managing your support desk from Claude, Cursor, or any MCP-compatible client

Your AI agent acts as a junior support representative, capable of summarizing long ticket threads and drafting professional responses.

### Who is this for?

- **Support Agents** — quickly summarize a 20-message thread and draft a reply without reading the entire history manually
- **Customer Success Managers** — check the status of high-priority tickets and add internal notes to guide the support team
- **E-commerce Managers** — quickly look up a customer's support history before reaching out for a sales call


## Available Tools
- **create_customer**: Create a new customer profile
- **create_message**: Add a message (reply or internal note) to a ticket
- **create_ticket**: Create a new ticket
- **get_customer**: Get details for a specific customer
- **get_ticket**: Get details of a specific ticket
- **get_user**: Get details for a specific agent/user
- **list_customers**: List or search customers
- **list_messages**: List messages within a ticket
- **list_tickets**: List support tickets
- **list_users**: List agents/users in the workspace
- **update_customer**: Update a customer profile
- **update_ticket**: Update an existing ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gorgias** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent open tickets."

**🤖 AI Agent:**
> Fetching tickets... You have 5 recent open tickets:
1. Ticket #1042: 'Where is my order?' from john@example.com
2. Ticket #1041: 'Refund request' from sarah@example.com
...
Would you like me to read the messages for Ticket #1042?

---

**👤 You:**
> "Reply to ticket #1042 saying their order has been shipped and provide the tracking link."

**🤖 AI Agent:**
> Drafting reply... I've successfully posted a message to Ticket #1042 informing John that his order is on the way with the tracking details. Should I close the ticket?

---

**👤 You:**
> "Check if there's a profile for customer alex.smith@example.com."

**🤖 AI Agent:**
> Checking customer records...
Yes, I found a matching profile. Customer ID: 90210. Alex Smith currently has 2 resolved past tickets and 0 active issues.


## Installation & Usage

To install and use the **Gorgias** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gorgias](https://vinkius.com/mcp/gorgias)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
