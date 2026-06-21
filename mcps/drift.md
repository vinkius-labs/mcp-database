# Drift MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drift)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/drift-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/drift-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent to manage conversations, track contacts, and monitor agent availability via the Drift API.

## Description
Integrate **Drift**, the leading conversational marketing and sales platform, directly into your AI workflow. Manage your customer conversations and transcripts, track identified contacts and their profile attributes, monitor agent availability and roles, and oversee your conversational playbooks using natural language.

### What you can do

- **Conversation Oversight** — List and retrieve detailed information and full transcripts for all your Drift customer interactions.
- **Contact Intelligence** — Monitor identified contacts, their email addresses, custom profile attributes, and organizational accounts.
- **Agent Management** — Track real-time agent availability statuses, presence, and organizational roles across your team.
- **Playbook Monitoring** — List all configured conversational playbooks (bots) and identify their current activation statuses.

### How it works

1. Connect the Drift integration to your AI assistant.
2. Authorize using your Drift Personal Access Token or OAuth Token.
3. Orchestrate your conversational marketing and customer engagement through intuitive conversation.

### Who is this for?

- **Sales Managers** — Quickly check recent conversation transcripts and agent responsiveness on the go.
- **Marketing Operations** — Monitor contact identification volumes and playbook statuses via chat.
- **Customer Success** — Research specific contact profiles and interaction history to assist customers instantly.


## Available Tools
- **get_drift_platform_metadata**: Retrieve metadata for the current authenticated Drift account
- **get_contact_profile**: Get full profile data and interaction history for a specific contact
- **get_conversation_details**: Get detailed information and full transcript for a specific conversation
- **quick_agent_availability_audit**: Retrieve a high-level summary of active agent availability statuses
- **list_drift_contacts**: List all contacts synchronized or identified in your Drift account
- **list_drift_conversations**: List all active and recent customer conversations in Drift
- **list_drift_playbooks**: List all configured conversational playbooks (bots)
- **list_latest_customer_interactions**: Identify the most recently updated customer conversations
- **list_drift_agents**: List all registered agents and users in your Drift organization
- **search_contacts_by_email**: Search for a contact using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Drift conversations."

**🤖 AI Agent:**
> I've found 5 active conversations, including interactions with 'John Doe' and 'Anonymous Visitor #123'. Would you like to see the transcript for the conversation with John Doe?

---

**👤 You:**
> "Show me the contact profile for 'robert.brown@example.org'."

**🤖 AI Agent:**
> Robert Brown is a known contact from 'Tech Corp'. He has had 3 previous conversations and was last seen 2 hours ago. His profile includes attributes for 'Job Title: CTO' and 'Location: London'. Should I pull his full interaction history?

---

**👤 You:**
> "Who is currently available to take chats in Drift?"

**🤖 AI Agent:**
> Currently, 3 agents are 'Available': 'Alice Johnson', 'Bob Miller', and 'Kenji Tanaka'. 2 other agents are 'Away'. Would you like to see the current conversation load for the available agents?


## Installation & Usage

To install and use the **Drift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drift](https://vinkius.com/mcp/drift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
