# Aventri MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aventri)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aventri-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aventri-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage events, contacts, and speakers via Aventri — list events, search contacts, and clone event modules directly from your AI agent.

## Description
Connect your **Aventri** (now Stova) account to any AI agent to streamline your event management and attendee coordination through natural language.

### What you can do

- **Event Management** — List all events, search for specific ones by name or date, and clone existing events including specific modules for rapid setup.
- **Contact & Attendee CRM** — Add, update, or delete contacts. Retrieve detailed profiles and search your database by email or unique identifiers.
- **Speaker Coordination** — List all account-level speakers, fetch detailed session associations, and create new speaker profiles instantly.
- **Pre-Approval Workflows** — Manage pre-load and pre-approved lists to ensure smooth registration and access control.

### How it works

1. Subscribe to this server
2. Enter your Aventri Account ID and API Key
3. Start orchestrating your conferences and meetings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — quickly duplicate successful event structures and manage speaker lists without manual data entry.
- **Marketing Operations** — sync contact data and manage attendee lists directly from your workflow tools.
- **Executive Assistants** — retrieve event details and speaker bios for briefings using simple conversational queries.


## Available Tools
- **add_contact**: Add a new contact to the account or database
- **add_pre_approved**: Add contacts to a pre-approved list
- **add_pre_load**: Add pre-load registrant data
- **clone_event**: Clone an existing event
- **create_speaker**: Create an account-level speaker
- **delete_contact**: Delete a contact from the system
- **get_contact**: Get detailed information for a specific contact
- **get_speaker**: Get speaker details and associated sessions
- **list_contacts**: List contacts in the Aventri account
- **list_events**: List all events in the account
- **list_speakers**: List all speakers associated with the account
- **search_events**: Search and filter events
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aventri** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all events currently in my Aventri account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 active events: 'Global Tech Summit 2024' (ID: 8821), 'Annual Partner Meetup' (ID: 9932), and 'Developer Workshop' (ID: 10443).

---

**👤 You:**
> "Find the contact details for the user with email 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching contacts... I found John Doe (Contact ID: 55402). He is registered as a 'Senior Manager' at 'Example Corp'. Would you like to see his full profile?

---

**👤 You:**
> "Clone event 8821 and call it 'Global Tech Summit 2025'."

**🤖 AI Agent:**
> I am initiating the clone process for event 8821. I will duplicate the core modules to create your new 2025 event instance. One moment...


## Installation & Usage

To install and use the **Aventri** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aventri](https://vinkius.com/mcp/aventri)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
