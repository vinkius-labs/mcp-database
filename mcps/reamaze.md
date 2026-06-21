# Reamaze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reamaze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reamaze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reamaze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer support and helpdesk workflows via Reamaze — manage help articles, channels, and contacts directly from any AI agent.

## Description
Connect your **Reamaze** account to any AI agent to streamline your customer support operations and knowledge base management through natural conversation.

### What you can do

- **Knowledge Base Management** — List, retrieve, create, and update help articles to keep your documentation synchronized.
- **Channel Oversight** — Inspect active support channels including email, chat, and social media integrations to understand your support surface.
- **Contact Management** — Search for customer profiles, create new contacts, and update existing user data to maintain a clean CRM.
- **Article Search** — Query your help center using keywords or status filters to find the exact information your customers need.

### How it works

1. Subscribe to this server
2. Enter your Reamaze Brand name, Login Email, and API Token
3. Start managing your support ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly audit help center content and monitor active communication channels.
- **Customer Success Managers** — update contact information and custom data fields without leaving the conversation.
- **Content Strategists** — draft and update help articles directly through AI assistance.


## Available Tools
- **create_article**: Create a new Help Article
- **create_contact_note**: Attach a note to a contact
- **create_contact**: Create a new contact
- **create_conversation**: Create a new conversation on behalf of a customer
- **create_identity**: Attach an identity to a contact
- **create_incident**: Create a new incident
- **create_message**: Create a new message under a specific conversation
- **create_response_template**: Create a new Response Template
- **create_staff**: Create a new staff user
- **delete_contact_note**: Delete a contact note
- **get_article**: Retrieve a specific Help Article
- **get_channel**: Retrieve a specific channel
- **get_conversation**: Retrieve a specific conversation
- **get_incident**: Retrieve a specific incident
- **get_report**: Retrieve a specific report
- **get_response_template**: Retrieve a specific Response Template
- **list_articles**: Can be scoped to a topic slug, filtered by status, or searched.

List Help Articles for the Brand
- **list_channels**: List channels for the Brand
- **list_contact_notes**: Retrieve notes for a specific contact
- **list_contacts**: List contacts for the Account
- **list_conversations**: List conversations for the Brand
- **list_identities**: Retrieve identities for a contact
- **list_incidents**: Retrieve incidents for the Brand
- **list_messages**: Retrieve individual messages for all conversations
- **list_response_templates**: Retrieve Response Templates for the Brand
- **list_satisfaction_ratings**: Retrieve satisfaction survey ratings
- **list_staff**: Retrieve staff users for the Account
- **list_systems**: Retrieve systems for the Brand
- **update_article**: Update a specific Help Article
- **update_contact_note**: Update a contact note
- **update_contact**: Update a specific contact
- **update_conversation**: Update a conversation
- **update_incident**: Update a specific incident
- **update_response_template**: Update a specific response template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reamaze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for help articles related to 'refund policy' and list them."

**🤖 AI Agent:**
> I found 2 articles matching 'refund policy': 'Standard Refund Procedure' (slug: standard-refund) and 'International Returns' (slug: international-returns). Would you like to see the content of one of them?

---

**👤 You:**
> "Create a new contact for John Doe with email john@example.com."

**🤖 AI Agent:**
> I have successfully created the contact for John Doe (john@example.com). The profile is now active in your Reamaze account.

---

**👤 You:**
> "List all active email channels for our brand."

**🤖 AI Agent:**
> I've retrieved your email channels. You have 2 active: 'Support Main' (support@brand.com) and 'Sales Inquiry' (sales@brand.com).


## Installation & Usage

To install and use the **Reamaze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reamaze](https://vinkius.com/mcp/reamaze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
