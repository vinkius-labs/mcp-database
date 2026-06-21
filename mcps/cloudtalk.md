# CloudTalk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudtalk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudtalk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudtalk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Modern cloud-based phone system designed for sales and support teams, offering seamless call center automation.

## Description
CloudTalk is a modern cloud-based phone system designed for sales and support teams, offering seamless call center automation and CRM integrations. It empowers agents to handle calls efficiently across the globe. You can easily fetch call logs, search contacts, and retrieve analytics metrics programmatically.


## Available Tools
- **create_contact**: Provide at least a name or email.

Create a new contact in CloudTalk
- **delete_contact**: Deletes the contact and all associated data.

Permanently remove a contact from CloudTalk
- **get_contact**: Retrieve detailed information about a specific contact
- **list_agents**: Retrieve a list of agents from CloudTalk
- **list_calls**: Supports filtering by agent and direction.

Retrieve a list of calls from CloudTalk
- **list_contacts**: Supports pagination and filtering by email or phone number.

Retrieve a list of contacts from CloudTalk
- **make_call**: Provide the from/to numbers.

Initiate a phone call between an agent and a destination number
- **update_contact**: Provide the contactId and any fields to update.

Update an existing contact in CloudTalk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudTalk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 calls in CloudTalk."

**🤖 AI Agent:**
> Here are the last 10 calls:
1. +1-555-0123 → Sales Team (4m 32s, completed)
2. +44-20-7946 → Support (2m 15s, completed)
3. +1-555-0456 → Marketing (missed)
... Showing 3 of 10. Total talk time: 28 minutes.

---

**👤 You:**
> "Find the contact with email 'john.doe@example.com' in CloudTalk."

**🤖 AI Agent:**
> Found contact: John Doe (john.doe@example.com). Phone: +1-555-0199. Company: Acme Corp. Agent: Sarah M. Last call: March 15, 2025 (3m 45s). Total interactions: 12.

---

**👤 You:**
> "Initiate a call to +123456789 from my CloudTalk extension."

**🤖 AI Agent:**
> Call initiated to +123456789 from your extension (ext. 204). Status: ringing. Call ID: call_8f3a2b. You'll receive a notification when the call connects.


## Installation & Usage

To install and use the **CloudTalk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudtalk](https://vinkius.com/mcp/cloudtalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
