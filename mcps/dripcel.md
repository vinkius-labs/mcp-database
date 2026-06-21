# Dripcel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dripcel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dripcel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dripcel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to manage WhatsApp instances, track contacts, and monitor messaging automation via the Dripcel API.

## Description
Integrate **Dripcel**, the powerful WhatsApp automation platform, directly into your AI workflow. Manage your WhatsApp instances and connection statuses, track identified contacts and phone numbers, monitor message history and templates, and oversee your messaging operations using natural language.

### What you can do

- **Instance Oversight** — List and retrieve detailed information and connection status for all your WhatsApp instances.
- **Contact Intelligence** — Monitor identified contacts, their phone numbers, and last interaction history across your organization.
- **Messaging Intelligence** — Monitor real-time messaging logs, delivery statuses, and approved templates via chat.
- **Automation Auditing** — Retrieve high-level summaries of instance activity, connection health, and active in-progress communications.

### How it works

1. Connect the Dripcel integration to your AI assistant.
2. Authorize using your Dripcel API Key (found in your account settings).
3. Orchestrate your WhatsApp automation and customer engagement through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check instance connection status and messaging volumes on the go.
- **Customer Engagement Leads** — Research contact profiles and interaction history via chat during campaigns.
- **IT Administrators** — Monitor automation instance health and API limits across the organization instantly.


## Available Tools
- **get_dripcel_account_metadata**: Retrieve metadata and limits for your Dripcel account
- **get_whatsapp_connection_status**: Identify if a specific WhatsApp instance is currently connected and authenticated
- **get_instance_details**: Get detailed settings and information for a specific WhatsApp instance
- **quick_instance_health_audit**: Retrieve a high-level summary of all instances and their connection states
- **list_instance_contacts**: List all contacts registered or identified within a specific WhatsApp instance
- **list_whatsapp_instances**: List all WhatsApp instances configured in your Dripcel account
- **list_whatsapp_messages**: List recent messages sent or received by a specific instance
- **list_whatsapp_templates**: List all message templates configured for a specific instance
- **search_instance_contacts**: Search for contacts within an instance using a keyword or phone number
- **send_whatsapp_message**: Send a text message via a specific WhatsApp instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dripcel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active WhatsApp instances."

**🤖 AI Agent:**
> I've found 3 active instances, including 'Main Office' (Connected) and 'Sales Team' (Connected). Would you like to see the connection status for the third instance?

---

**👤 You:**
> "Send message 'Your order is ready' to '+1 555-0123' via instance 'main_inst'."

**🤖 AI Agent:**
> I've successfully sent the message 'Your order is ready' to +1 555-0123. The message ID is 'DRIP-MSG-7788'. Should I check the delivery status for you in a moment?

---

**👤 You:**
> "Check the connection health for instance 'sales_inst'."

**🤖 AI Agent:**
> Instance 'sales_inst' is currently 'Connected' and authenticated. Battery level is at 85% and signal strength is strong. Should I list the most recent messages for this instance?


## Installation & Usage

To install and use the **Dripcel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dripcel](https://vinkius.com/mcp/dripcel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
