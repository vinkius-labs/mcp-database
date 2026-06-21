# Polaria MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polaria)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/polaria-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/polaria-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Unify your customer support with an AI agent that manages Polaria conversations, contacts, and FAQ retrieval.

## Description
Transform your customer support operations by connecting Polaria directly to your AI agent. Let your assistant automatically retrieve relevant help articles, instantly respond to customer conversations, and efficiently manage your user directory without navigating away from your central workspace.

### What you can do
- Access and organize your entire customer contact database
- Read and respond to live chat conversations instantly
- Update the status of support tickets (Open, Pending, Resolved)
- Retrieve FAQ articles to resolve customer inquiries faster
- Manage custom attributes for targeted support

### How it works
1. Log into your Polaria dashboard
2. Create a new app under Settings > Marketplace to get your Secret Key
3. Connect via Vinkius to unleash AI-powered conversational support

### Who is it for?
Ideal for customer success teams, support agents, and community managers who want to resolve user queries faster and automate repetitive chat tasks.


## Available Tools
- **create_contact**: Create a new contact in Polaria
- **add_chat_message**: Add a message to a conversation
- **get_contact**: Get details of a specific contact
- **get_conversation**: Get details of a specific conversation
- **list_contacts**: List contacts in Polaria
- **list_conversations**: List conversations in Polaria
- **list_faqs**: List FAQs in Polaria
- **list_widgets**: List Polaria widgets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polaria** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in Polaria."

**🤖 AI Agent:**
> You have 1,240 contacts in Polaria. Would you like me to filter them by a specific segment or recent activity?

---

**👤 You:**
> "Show recent chat conversations."

**🤖 AI Agent:**
> Here are the 3 most recent chat conversations: 1) Billing issue with John Doe (Open), 2) Refund request from Acme Corp (Pending), 3) Technical support for Sarah (Resolved).

---

**👤 You:**
> "Add a reply message to conversation 'C123'."

**🤖 AI Agent:**
> I've successfully added your reply to conversation 'C123' and marked the status as 'Waiting on Customer'.


## Installation & Usage

To install and use the **Polaria** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polaria](https://vinkius.com/mcp/polaria)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
