# SimpleTexting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simpletexting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/simpletexting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/simpletexting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send mass text messages, run SMS campaigns, and manage two-way conversations with customers from one simple platform.

## Description
Connect your **SimpleTexting** account to any AI agent and take full control of your business text messaging and mass SMS orchestration through natural conversation. SimpleTexting provides a premier platform for text marketing and customer communication, and this integration allows you to send messages, manage contact lists, and monitor conversational history directly from your chat interface.

### What you can do

- **Messaging Orchestration** — Send instant or scheduled SMS messages to individual contacts or broadcast lists programmatically.
- **Contact & List Management** — Create, update, and manage your subscriber database and segments directly from the AI interface.
- **Conversation Intelligence** — Access and monitor real-time text conversations to maintain high-quality customer engagement via natural language.
- **Autoresponder & Template Control** — Access available messaging lists and monitor autoresponders to ensure your automated flows are optimized.
- **Operational Monitoring** — Retrieve account profile metadata and monitor delivery statuses via simple AI commands to ensure reliable outreach.

### How it works

1. Subscribe to this server
2. Enter your SimpleTexting API v2 Token from your account settings
3. Start managing your SMS marketing from Claude, Cursor, or any MCP-compatible client

No more manual typing or list exporting. Your AI acts as a dedicated marketing manager or customer engagement coordinator.

### Who is this for?

- **Marketing Managers** — quickly send promotional SMS and monitor campaign delivery without manual exports.
- **Customer Support Teams** — automate the retrieval of conversation history and respond to clients via natural language.
- **Operations Teams** — streamline the management of contact segments and monitor list growth directly within the chat.


## Available Tools
- **create_subscriber**: Add new contact
- **remove_subscriber**: Delete contact
- **get_api_status**: Check connection
- **get_subscriber_details**: Get contact info
- **list_subscribers**: List SMS contacts
- **list_chat_conversations**: Get message history
- **list_contact_lists**: List static groups
- **list_audience_segments**: List dynamic segments
- **list_active_webhooks**: Get event configs
- **schedule_sms_delivery**: Schedule future SMS
- **send_sms_message**: Send text message
- **update_subscriber_info**: Modify contact data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimpleTexting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS broadcast to the 'New Arrivals' list: 'Check out our new collection!'."

**🤖 AI Agent:**
> SMS broadcast triggered! I've sent the message to all 150 contacts in your 'New Arrivals' list via SimpleTexting.

---

**👤 You:**
> "Schedule a text to +1234567890 for tomorrow at 10 AM saying 'Don't forget our meeting'."

**🤖 AI Agent:**
> Message scheduled! I've set the SMS to be delivered to +1234567890 at the specified time. Would you like to see your other pending scheduled messages?

---

**👤 You:**
> "Search for a contact with phone number +1987654321."

**🤖 AI Agent:**
> Searching contacts... I found 'Alice Cooper' associated with that number. She is in the 'VIP' list and has received 3 messages recently. Should I retrieve her full interaction history?


## Installation & Usage

To install and use the **SimpleTexting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simpletexting](https://vinkius.com/mcp/simpletexting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
