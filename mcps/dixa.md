# Dixa MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dixa)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dixa-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dixa-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage customer conversations, track agents, and monitor support queues via the Dixa API.

## Description
Integrate **Dixa**, the customer friendship platform, directly into your AI workflow. Manage your multi-channel support conversations, monitor agent presence and performance, track service queues, and oversee your support teams using natural language.

### What you can do

- **Conversation Oversight** — List and retrieve detailed information for all customer conversations and their current processing status.
- **Agent Intelligence** — Monitor real-time agent presence, profile details, and team assignments across your organization.
- **Queue Monitoring** — Track active service queues and routing settings to ensure efficient support delivery.
- **Team Management** — List all support teams and identify members assigned to specific organizational units.

### How it works

1. Connect the Dixa integration to your AI assistant.
2. Authorize using your Dixa API Token (found in your organization settings).
3. Orchestrate your customer service and support operations through intuitive conversation.

### Who is this for?

- **Support Managers** — Quickly check queue volumes and agent availability on the go.
- **Customer Success Leads** — Research conversation history and agent performance via chat.
- **Operations Teams** — Monitor support team structures and organizational metadata instantly.


## Available Tools
- **get_service_account_metadata**: Retrieve metadata and usage limits for your Dixa account
- **get_agent_profile**: Get full profile and performance data for a specific agent
- **get_conversation_details**: Get detailed information for a specific customer conversation
- **quick_agent_presence_audit**: Retrieve a high-level summary of active agent presence statuses
- **list_service_agents**: List all support agents registered in your Dixa organization
- **list_customer_conversations**: List all customer service conversations in your Dixa account
- **list_open_support_tickets**: Identify conversations that are currently in an "Open" or "Unassigned" status
- **list_service_queues**: List all active service queues configured in Dixa
- **list_support_teams**: List all configured support teams and their members
- **search_conversations_by_subject**: Search for conversations using a keyword in the subject


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dixa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open support conversations."

**🤖 AI Agent:**
> I've found 8 open conversations, including 'Issues with Payment' and 'Feature Request: Dark Mode'. Would you like to see the assigned agent for any of these?

---

**👤 You:**
> "Show me the details for conversation '12345'."

**🤖 AI Agent:**
> Conversation '12345' (Subject: Login Issue) is currently 'Open' and assigned to 'John Doe'. It was created 2 hours ago via Email. Should I pull the latest message from this conversation?

---

**👤 You:**
> "Who is currently available in the 'Sales' team?"

**🤖 AI Agent:**
> In the Sales team, 3 agents are currently 'Available': 'Alice Johnson', 'Bob Miller', and 'Kenji Tanaka'. 2 other members are 'Away'. Would you like to see the current load for the available agents?


## Installation & Usage

To install and use the **Dixa** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dixa](https://vinkius.com/mcp/dixa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
