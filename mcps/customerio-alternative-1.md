# Customer.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customerio-alternative-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/customerio-alternative-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/customerio-alternative-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate customer engagement via Customer.io — track events, manage profiles, and trigger multi-channel campaigns directly from any AI agent.

## Description
Connect your **Customer.io** account to any AI agent to orchestrate sophisticated marketing automation and transactional messaging through natural language.

### What you can do

- **Profile Management** — Create, update, or delete customer profiles and merge duplicate identities using the Track API.
- **Event Tracking** — Record custom events for identified or anonymous users to trigger behavioral workflows.
- **Campaign Orchestration** — Trigger API-triggered broadcasts and send newsletters to specific segments instantly.
- **Transactional Messaging** — Send high-priority transactional emails, push notifications, and in-app messages with custom data payloads.
- **Data Pipeline** — Leverage the Pipeline API to identify users, track pages, screens, and groups across your entire stack.

### How it works

1. Subscribe to this server
2. Enter your Customer.io Site ID, API Key, and App API Key
3. Start managing your customer lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — trigger campaigns and update user segments without touching code or CSV exports.
- **Product Managers** — track new feature adoption events and analyze user behavior directly through the AI.
- **Support & Ops** — manually update customer attributes or trigger transactional receipts during troubleshooting sessions.


## Available Tools
- **add_or_update_customer**: Add or update a person (v1)
- **delete_customer**: Delete a person (v1)
- **merge_customers**: Merge two customer profiles (v1)
- **pipeline_batch**: Send multiple calls in a single request (Pipelines API)
- **pipeline_group**: Associate people with objects like companies (Pipelines API)
- **pipeline_identify**: Identify a person and assign traits (Pipelines API)
- **pipeline_page**: Record page views (Pipelines API)
- **pipeline_screen**: Record mobile screen views (Pipelines API)
- **pipeline_track**: Record actions people take (Pipelines API)
- **send_newsletter**: Send a newsletter immediately
- **send_transactional_email**: Send a transactional email
- **send_transactional_in_app**: Send a transactional in-app message
- **send_transactional_push**: Send a transactional push notification
- **track_anonymous_event**: Send anonymous events (v1)
- **track_batch**: Send multiple entity operations in one request (v2)
- **track_customer_event**: Track an event for a person (v1)
- **track_entity**: Create, update, or delete a single person or object (v2)
- **trigger_broadcast**: Trigger an API-triggered broadcast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update customer 'user_123' and set their 'loyalty_tier' to 'gold'."

**🤖 AI Agent:**
> I've updated the profile for 'user_123'. Their 'loyalty_tier' is now set to 'gold' in Customer.io.

---

**👤 You:**
> "Track a 'completed_tutorial' event for customer 'jane@example.com'."

**🤖 AI Agent:**
> The 'completed_tutorial' event has been successfully recorded for jane@example.com.

---

**👤 You:**
> "Send a transactional email using template ID 'welcome_msg' to 'new_user@test.com'."

**🤖 AI Agent:**
> I've triggered the transactional email 'welcome_msg' for new_user@test.com via the App API.


## Installation & Usage

To install and use the **Customer.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customerio-alternative-1](https://vinkius.com/mcp/customerio-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
