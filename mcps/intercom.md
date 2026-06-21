# Intercom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/intercom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/intercom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/intercom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Equip your AI agent with direct access to Intercom — manage conversations, search contacts, and track customer data without opening the Intercom inbox.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intercom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the contact record for sarah@startup.io."

**🤖 AI Agent:**
> Found: Sarah Chen (sarah@startup.io). Company: Startup.io (Growth plan). Last seen: 2 hours ago. Total conversations: 12 (3 open). Custom attributes: MRR $2,400, Account Manager: James.

---

**👤 You:**
> "How many open conversations do we have right now?"

**🤖 AI Agent:**
> You currently have 23 open conversations. Breakdown: 8 unassigned, 10 assigned to support agents, and 5 snoozed. The oldest open conversation is 4 hours old (assigned to Maria).

---

**👤 You:**
> "List all companies on our Enterprise plan."

**🤖 AI Agent:**
> I found 14 companies on the Enterprise plan. Top 5 by user count: Acme Corp (250 users), GlobalTech (180 users), DataFlow Inc (95 users), CloudFirst (72 users), and SecureStack (45 users).


## Installation & Usage

To install and use the **Intercom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intercom](https://vinkius.com/mcp/intercom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
