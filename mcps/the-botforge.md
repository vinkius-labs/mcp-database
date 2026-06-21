# The Botforge MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-botforge)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/the-botforge-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/the-botforge-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deploy custom AI chatbots for enterprise customer support with multilingual capability and deep integration into your tech stack.

## Description
Connect your **The Botforge** account to any AI agent and simplify how you manage your conversational AI, handle contact submissions, and monitor bot health through natural conversation.

### What you can do

- **Bot Oversight** — List all chatbots in your account and retrieve real-time operational status for specific bot IDs.
- **Contact Submission** — Programmatically submit data to your bot's contact forms, ideal for automated lead capture.
- **Event Integration** — Subscribe to bot events via webhooks to receive real-time updates on user interactions.
- **Metadata Inspection** — Retrieve sample data and form field configurations to understand your bot's data structure.
- **Operational Monitoring** — Check connectivity and verify if your bots are online and responsive via AI queries.

### How it works

1. Subscribe to this server
2. Enter your The Botforge API Key (found in your account dashboard)
3. Start managing your conversational ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Chatbot Developers** — quickly check bot statuses and test form submissions via simple AI commands.
- **Marketing Teams** — automate lead capture from external sources directly into your bot engine.
- **Support Managers** — monitor bot health and receive real-time interaction events without leaving the workspace.


## Available Tools
- **get_bot_status**: Check bot operational status
- **get_samples**: Get bot form field samples
- **list_bots**: List all chatbots
- **submit_contact**: Pass data as a JSON string.

Submit data to the bot contact form
- **subscribe_webhook**: Pass data as a JSON string.

Subscribe to bot events via webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Botforge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all chatbots in my account."

**🤖 AI Agent:**
> I've retrieved your chatbots. You have 3 active bots including 'Customer Support', 'Sales Assistant', and 'Lead Intake'. Which one would you like to check the status for?

---

**👤 You:**
> "Submit a contact to the bot: { "first_name": "John", "email": "john@example.com", "message": "Interested in a demo" }."

**🤖 AI Agent:**
> Submission successful! I've sent the contact details for John (john@example.com) to your bot engine. The data has been logged correctly.

---

**👤 You:**
> "Check the operational status of bot 'bot_10293'."

**🤖 AI Agent:**
> Fetching status... Bot bot_10293 ('Customer Support') is currently 'Online' and responding normally. Last interaction was recorded 5 minutes ago.


## Installation & Usage

To install and use the **The Botforge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-botforge](https://vinkius.com/mcp/the-botforge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
