# Messenger MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messenger)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/messenger-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/messenger-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Control and manage your Facebook Page conversations — audit messages and personas via AI.

## Description
Empower your AI agent to orchestrate your entire mobile communication strategy on **Facebook Messenger**, the leading platform for social engagement. By connecting Messenger to your agent, you transform enterprise messaging into a natural conversation. Your agent can instantly list your conversations, audit message history, and send replies without you ever touching a complex Meta dashboard. Whether you are providing customer support or managing brand personas, your agent acts as a real-time communication assistant, ensuring your Page is always responsive and your community data is organized.

### What you can do

- **Conversation Auditing** — List all active conversations for your Page and retrieve detailed message history including timestamps.
- **Messaging Intelligence** — Send direct text replies to users instantly to maintain a high response rate.
- **Persona Oversight** — List and retrieve information for brand personas to ensure your bot's identity is correctly applied.
- **Page Governance** — Monitor Page settings and info to maintain strict organizational control over your brand presence.
- **Content Insights** — List message creatives to ensure your automated responses are using the correct media assets.

### How it works

1. Subscribe to this server
2. Enter your Facebook Page Access Token and Page ID
3. Start managing your Messenger interactions through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — monitor user inquiries and send quick updates straight from your workflow.
- **Marketing Leads** — verify if new personas and message creatives have been correctly configured.
- **Social Media Managers** — perform rapid audits of conversation threads without manual Meta logins.
- **Operations Managers** — automate messaging workflows to orchestrate customer engagement smoothly.


## Available Tools
- **get_messages**: Get message history for a specific conversation
- **get_page_info**: Get basic information about the connected Facebook Page
- **get_page_settings**: Get settings for the Facebook Page
- **get_persona_info**: Get details for a specific persona
- **list_conversations**: List recent Messenger conversations for the page
- **list_message_creative**: List message creatives for the page
- **list_personas**: List all personas for the page
- **send_message**: Send a text message reply to a recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Messenger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Messenger conversations for my Page."

**🤖 AI Agent:**
> I've retrieved your conversations. You have 5 recent threads, including interactions with 'John Doe' and 'Jane Smith'. Which conversation ID would you like to audit for history?

---

**👤 You:**
> "Send 'Thank you for contacting us!' to recipient ID 12345678."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your reply to recipient 12345678. The response is now visible in the Messenger thread.

---

**👤 You:**
> "Show me the message history for conversation t_xxxx."

**🤖 AI Agent:**
> I've retrieved the history for t_xxxx. There are 10 messages in this thread. The latest was 'Hello, I have a question about my order' from the user. Would you like the full log?


## Installation & Usage

To install and use the **Messenger** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messenger](https://vinkius.com/mcp/messenger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
