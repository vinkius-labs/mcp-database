# ChatGen MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatgen)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chatgen-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chatgen-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Convert website visitors into qualified leads with AI chatbots that engage, qualify, and route prospects in real time.

## Description
Connect your **ChatGen** account to any AI agent and simplify your conversational marketing and lead management through natural conversation.

### What you can do

- **Bot Management** — List all your chatbots, retrieve detailed configuration metadata, and create or update bots programmatically
- **Lead Generation** — Query and analyze leads captured by your bots to sync with your sales workflows
- **Conversation Tracking** — Monitor recent chat sessions to understand user interactions and bot performance
- **Team Insights** — List organizational teams to understand your account structure

### How it works

1. Subscribe to this server
2. Enter your ChatGen API Key from your dashboard
3. Start managing your chatbot resources from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_bot**: Create a new chatbot
- **delete_bot**: Delete a bot
- **get_bot**: Get details for a specific bot
- **get_lead_details**: Get details for a specific lead
- **list_bots**: List all ChatGen bots
- **list_conversations**: List recent bot conversations
- **list_leads**: List captured leads
- **list_teams**: List organizational teams
- **update_bot**: Update an existing bot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChatGen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my ChatGen bots."

**🤖 AI Agent:**
> I've retrieved your bots. You have 3 bots: 'Sales Bot', 'Support Assistant', and 'Lead Gen 2024'.

---

**👤 You:**
> "Show me details for the lead 'lead_999'."

**🤖 AI Agent:**
> Lead 'lead_999' is Robert Fox (robert@example.com). They were captured by the 'Sales Bot' and expressed interest in the Enterprise plan.

---

**👤 You:**
> "Find recent bot conversations."

**🤖 AI Agent:**
> I found 10 recent conversations. Most users are asking about pricing and integration options. Would you like a summary of the latest one?


## Installation & Usage

To install and use the **ChatGen** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatgen](https://vinkius.com/mcp/chatgen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
