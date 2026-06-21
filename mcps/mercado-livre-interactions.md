# Mercado Livre Interactions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-livre-interactions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mercado-livre-interactions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mercado-livre-interactions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Answer buyer questions, check reputation, and view metrics on Mercado Livre.

## Description
Connect **Mercado Livre Interactions** to any AI agent and manage your seller reputation — answer questions, view performance metrics, and handle buyer communication through natural conversation.

### What you can do
- **Questions & Answers** — List unanswered questions and respond to buyers instantly
- **Reputation Check** — Monitor your seller reputation level (Green, Yellow, Red)
- **Performance Metrics** — View late shipments, cancellations, and claim rates
- **Message History** — Access communication logs with buyers for specific orders

### How it works
1. Subscribe to this server
2. Enter your Mercado Livre OAuth2 Access Token
3. Start managing interactions from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Sellers** — Improve response times to buyer questions and maintain a healthy reputation
- **Support Teams** — Quickly check order history and communication logs
- **Brand Managers** — Monitor seller metrics to ensure high performance standards


## Available Tools
- **answer_question**: Reply to a buyer's question
- **get_messages**: Get message history for a sale
- **get_metrics**: Get detailed seller metrics
- **get_questions**: Optional item_id to filter.

List unanswered questions from buyers
- **get_reputation**: Get seller reputation level and metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Livre Interactions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my unanswered questions."

**🤖 AI Agent:**
> Found 2 unanswered questions: 1. 'Does it come with a charger?'. 2. 'Is it compatible with iPhone 15?'.

---

**👤 You:**
> "Answer question 999 with 'Yes, it includes the original charger.'"

**🤖 AI Agent:**
> Answer sent successfully! The buyer will receive a notification.

---

**👤 You:**
> "Check my seller reputation and metrics."

**🤖 AI Agent:**
> Reputation Level: Green (MercadoLíder). Metrics: Late shipments 2%, Cancellations 1%, Claims 0.5%.


## Installation & Usage

To install and use the **Mercado Livre Interactions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-livre-interactions](https://vinkius.com/mcp/mercado-livre-interactions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
