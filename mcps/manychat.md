# ManyChat MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/manychat)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/manychat-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/manychat-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate messenger marketing via ManyChat — manage subscribers, tags, and flows directly from any AI agent.

## Description
Connect your **ManyChat** account to any AI agent and take full control of your messenger marketing automation through natural conversation.

### What you can do

- **Subscriber Management** — Get detailed info, find subscribers by name or custom fields
- **Tagging** — Add or remove tags to segment your audience on the fly
- **Flow Automation** — Send specific flows to subscribers or list available flows
- **Custom Fields** — Set and query custom field values for personalized interactions

### How it works

1. Subscribe to this server
2. Enter your ManyChat API Token
3. Start managing your automations from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **add_tag**: Add a tag to a subscriber
- **find_subscriber_by_custom_field**: Find subscribers by custom field value
- **find_subscriber_by_name**: Find subscribers by name
- **get_subscriber_flows**: Get all flows assigned to a subscriber
- **get_subscriber_info**: Get subscriber information by ID
- **get_subscriber_tags**: Get all tags assigned to a subscriber
- **list_custom_fields**: List all custom fields on the page
- **list_tags**: List all tags on the page
- **remove_tag**: Remove a tag from a subscriber
- **send_flow**: Send a flow to a subscriber
- **set_custom_field**: Set a custom field value for a subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ManyChat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find subscriber info for ID 12345678."

**🤖 AI Agent:**
> I've retrieved the info for subscriber 12345678. Name: John Doe, Gender: male, Status: active.

---

**👤 You:**
> "Add the 'VIP' tag to subscriber 12345678."

**🤖 AI Agent:**
> The 'VIP' tag (ID: 987) has been successfully added to subscriber 12345678.

---

**👤 You:**
> "List all tags on my ManyChat page."

**🤖 AI Agent:**
> Here are the tags for your page: 'VIP', 'New Lead', 'Follow-up'.


## Installation & Usage

To install and use the **ManyChat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manychat](https://vinkius.com/mcp/manychat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
