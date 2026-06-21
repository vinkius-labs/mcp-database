# Formilla MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formilla)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/formilla-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/formilla-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Chat with website visitors in real time and use AI chatbots to qualify leads and answer common questions automatically.

## Description
Connect your **Formilla** account to any AI agent and take full control of your live chat contacts and customer data management through natural conversation.

### What you can do

- **Contact Orchestration** — Create or update contact records programmatically, including managing names, emails, and phone numbers directly from your agent
- **Database Management** — List all contacts in your Formilla account and retrieve detailed metadata to maintain a high-fidelity customer record
- **Visitor Intelligence** — Find specific contacts by email to verify their support history and track custom attributes for personalized messaging
- **Secure Maintenance** — Programmatically delete contacts from the system to maintain database hygiene and comply with privacy requests
- **Data Synchronization** — Use unique identifiers (UserId) to seamlessly sync your external user data with Formilla's live chat ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Auth Token** from your Formilla dashboard (Settings > Security)
3. Start managing your live chat contacts from Claude, Cursor, or any MCP client

No more manual data entry into the live chat dashboard. Your AI acts as your dedicated contact and data sync coordinator.

### Who is this for?

- **Support Teams** — instantly retrieve customer profiles and update contact info while managing live chats
- **Marketing Automators** — sync new leads and track custom attributes across your customer database using natural language
- **Operations Managers** — manage database hygiene and privacy compliance through automated contact deletion queries


## Available Tools
- **check_formilla_status**: Verify connectivity
- **delete_contact**: Delete a contact
- **get_contact_by_email**: Get contact by email
- **get_contact**: Get contact details
- **get_conversation**: Get conversation details
- **list_contacts**: List contacts
- **list_conversations**: List conversations
- **list_segments**: List segments
- **list_visitors**: List visitors
- **search_contacts**: Search contacts
- **update_contact**: Update a contact
- **upsert_contact**: Create or update contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formilla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current contacts in Formilla."

**🤖 AI Agent:**
> I've retrieved your contact list. You have 150 registered users. Recent additions include 'John Doe' (john@example.com) and 'Sarah Smith'. Would you like to check the details for any specific contact?

---

**👤 You:**
> "Update contact 'john@example.com' with phone '+15551234567'."

**🤖 AI Agent:**
> Done! I've updated the phone number for John Doe (john@example.com) in your Formilla account. The new details are now synced and available in your chat dashboard.

---

**👤 You:**
> "Find the contact details for 'sarah.smith@example.com'."

**🤖 AI Agent:**
> I've located Sarah Smith's profile (ID: frm_987). She is an active user with 3 past chat interactions. Her current attributes include 'Plan: Premium' and 'Region: US'. Shall I retrieve her full history?


## Installation & Usage

To install and use the **Formilla** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formilla](https://vinkius.com/mcp/formilla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
