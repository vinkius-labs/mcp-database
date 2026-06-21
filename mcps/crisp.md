# Crisp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crisp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crisp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crisp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Chat with website visitors in real time, manage support conversations, and build a knowledge base that reduces ticket volume.

## Description
Connect your **Crisp** account to any AI agent and take full control of your multi-channel customer support and visitor engagement workflows through natural conversation.

### What you can do

- **Conversation Orchestration** — List and manage active chat and email support sessions programmatically, including monitoring unread counts and conversation status in real-time
- **Automated Messaging** — Programmatically dispatch text messages to active sessions to coordinate immediate customer assistance and engagement
- **Thread Intelligence** — Access complete message histories for any session to provide high-fidelity context for your support and marketing responses
- **Visitor Lifecycle** — Retrieve detailed visitor profiles and people records to maintain a perfectly coordinated relationship history
- **Operational Monitoring** — Access real-time website traffic metrics and support volume summaries directly through your agent for instant CX reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Plugin ID**, **Plugin Key**, and **Website ID** from the Crisp dashboard
3. Start managing your omnichannel support from Claude, Cursor, or any MCP client

No more manual ticket shuffling or missing messages in busy chat windows. Your AI acts as your dedicated support engineer and visitor engagement coordinator.

### Who is this for?

- **Support Teams** — instantly respond to visitor queries and summarize conversation threads using natural language commands
- **Customer Success** — monitor visitor engagement and retrieve high-fidelity profile metadata without leaving your workspace
- **Growth Marketers** — automate personalized outreach to active visitors and track website traffic through simple AI queries


## Available Tools
- **get_conversation**: Get conversation details
- **get_messages**: List messages in a conversation
- **get_visitor_profile**: Get visitor profile details
- **list_conversations**: List all website conversations
- **list_visitors**: List all website visitors/people
- **send_message**: Pass data as a JSON string.

Send a message to a conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crisp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations on my website."

**🤖 AI Agent:**
> I've retrieved your active conversations. You have 3 open chats, including an inquiry from 'John' and a question about 'Premium Features'. Would you like the message history for any of these?

---

**👤 You:**
> "Show the transcript for chat session 'sess_123'."

**🤖 AI Agent:**
> Fetching transcript... Session sess_123 details a discussion about 'Setup Guides'. The visitor requested a link to the documentation, and Agent Sarah replied 10 minutes ago. Shall I draft a follow-up?

---

**👤 You:**
> "Find the visitor profile for 'jane@example.com'."

**🤖 AI Agent:**
> I've located Jane's profile. She has visited the pricing page 3 times today and is currently tagged as a 'VIP Lead'. Would you like to see her full conversation history?


## Installation & Usage

To install and use the **Crisp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crisp](https://vinkius.com/mcp/crisp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
