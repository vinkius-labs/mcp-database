# Aircall MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aircall)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aircall-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aircall-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Cloud business phone system — manage calls, contacts, and team availability via AI.

## Description
Connect your **Aircall** account to your AI agent to unlock professional voice orchestration and communication management. From auditing call logs and recordings to managing shared contacts and monitoring team availability, your agent handles your phone system through natural conversation.

### What you can do

- **Call Orchestration** — List and retrieve details for calls, including recordings, durations, and participant metadata
- **Contact Management** — Create, update, and search for shared or private contacts within your Aircall account
- **Team Oversight** — List users and teams to check availability statuses and departmental assignments
- **Number Auditing** — Retrieve details for your Aircall phone numbers, including their technical configurations
- **Communication Insights** — Quickly identify call trends or lookup contact history directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Aircall API ID and API Token
3. Start managing your communication platform and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Support Teams** — research contact history and update CRM data after important calls
- **Managers** — audit team call volumes and monitor availability patterns effortlessly
- **Operations Leads** — manage phone number assignments and verify system configurations via simple commands
- **Customer Success** — quickly look up call recordings and participant details to resolve complex inquiries


## Available Tools
- **list_calls**: List call logs
- **get_call_details**: Get call technical details
- **list_contacts**: List Aircall contacts
- **search_contacts**: Search contacts by phone
- **create_contact**: Add a new contact
- **list_users**: List team members
- **get_user_details**: Get user availability
- **list_numbers**: List phone numbers
- **get_number_details**: Get number configuration
- **list_teams**: List Aircall teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aircall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 calls made by my team."

**🤖 AI Agent:**
> I've retrieved your recent calls. You had 10 calls in the last hour, with an average duration of 4 minutes. 3 were inbound and 7 were outbound. Would you like to see the recordings for any of them?

---

**👤 You:**
> "Search for a contact with name 'John Doe'."

**🤖 AI Agent:**
> I've found 2 contacts matching 'John Doe'. One is at 'Future Corp' and the other is a private contact. Which one would you like to see the details for?

---

**👤 You:**
> "Check if user 'Jane Smith' is currently available for calls."

**🤖 AI Agent:**
> I've checked Jane Smith's status. She is currently 'Busy' on another call. Her average call duration is 5 minutes, so she might be free soon. Would you like me to check again in a moment?


## Installation & Usage

To install and use the **Aircall** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aircall](https://vinkius.com/mcp/aircall)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
