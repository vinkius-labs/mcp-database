# Intercom MCP Server

Equip your AI agent with direct access to Intercom — manage conversations, search contacts, and track customer data without opening the Intercom inbox.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/intercom)

## Overview
**Category:** talk-to-me
**Tools Count:** 15

## Description
Connect **Intercom** to your AI agent and manage your customer communications and support operations conversationally.

### What you can do

- **Conversation Management** — List, search, and manage customer conversations with status, assignment, and SLA data.
- **Contact Search** — Query your customer database by email, name, company, or custom attributes to find specific users.
- **Company Data** — Retrieve company profiles, plan information, and aggregate usage metrics.
- **Support Analytics** — Pull conversation counts, response times, and resolution metrics for team performance reviews.

### How it works

1. Subscribe to the Intercom integration on the marketplace.
2. Create a private app in the Intercom Developer Hub and copy the Access Token.
3. Ask your AI agent to search contacts, list conversations, or pull customer data.

### Who is this for?

- **Customer Support Teams** — Get instant answers about customer history and conversation context without switching between tools.
- **Customer Success Managers** — Look up account health, usage patterns, and recent support interactions from your AI agent.
- **Sales Teams** — Pull contact and company data from Intercom to enrich leads and inform outreach strategies.


## Available Tools
- **create_contact**: Pass role (user/lead), email, and optional name. Returns the new contact ID.

Create a new contact/lead in Intercom
- **update_contact**: Pass the contact ID and a JSON body of fields to update.

Update an existing Intercom contact
- **assign_conversation**: Assign a conversation to a team member
- **close_conversation**: Requires the admin ID who is closing it.

Close/resolve a support conversation
- **list_conversations**: List all conversations
- **list_contacts**: List all contacts/leads
- **list_tags**: List all tags
- **list_segments**: List all user segments
- **get_contact**: Get contact details
- **search_contacts**: Search contacts by criteria
- **get_conversation**: Get conversation thread
- **reply_to_conversation**: Reply to a conversation
- **list_companies**: List all companies
- **list_articles**: List help center articles
- **list_admins**: List team members


## Installation & Usage

To install and use the **Intercom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intercom](https://vinkius.com/mcp/intercom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
