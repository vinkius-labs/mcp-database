# AI Receptionist MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-receptionist)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ai-receptionist-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ai-receptionist-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Let AI answer your business calls, book appointments, and handle customer inquiries around the clock without missing a beat.

## Description
Connect your **AI Receptionist** account to any AI agent and take full control of your automated customer engagement and front-desk workflows through natural conversation.

### What you can do

- **Conversation Orchestration** — List and monitor inbound and outbound AI voice or chat interactions programmatically, retrieving complete high-fidelity transcripts and operational metadata in real-time
- **Booking & Appointment Intelligence** — Access your complete directory of active appointments and programmatically create or manage bookings to maintain a perfectly coordinated schedule
- **Knowledge Base Discovery** — Access and monitor your organizational business rules and FAQs (Knowledge Base) to coordinate how your AI receptionist interacts with clients
- **Lead & Performance Intelligence** — Retrieve high-fidelity analytics on lead capture and interaction performance directly through your agent for instant operational reporting
- **Infrastructure Monitoring** — Verify API connectivity, access account metadata, and monitor active webhooks to maintain a perfectly coordinated communication ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AI Receptionist dashboard (Developer Settings > API)
3. Start orchestrating your automated front-desk from Claude, Cursor, or any MCP client

No more manual listening to call recordings or digging through individual lead tables. Your AI acts as your dedicated front-desk coordinator and interaction architect.

### Who is this for?

- **Business Owners** — instantly retrieve lead summaries and monitor AI performance using natural language commands
- **Operations Managers** — manage appointment schedules and verify knowledge base accuracy without leaving your workspace
- **Developers** — integrate high-speed AI voice intelligence and booking data into custom business workflows through simple AI queries


## Available Tools
- **create_aireceptionist_booking**: Create a booking
- **create_aireceptionist_conversation**: Create a new conversation
- **get_aireceptionist_analytics**: Get performance analytics
- **get_aireceptionist_booking**: Get booking details
- **get_aireceptionist_conversation**: Get conversation details
- **get_aireceptionist_me**: Get current user profile
- **list_aireceptionist_bookings**: List active bookings
- **list_aireceptionist_conversations**: List AI conversations
- **list_aireceptionist_knowledge**: List knowledge base articles
- **list_aireceptionist_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Receptionist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 conversations handled by the AI Receptionist."

**🤖 AI Agent:**
> I've retrieved your recent interactions. The last 5 conversations include 3 voice calls for 'Booking Inquiries' and 2 chat sessions. Would you like the detailed transcript for any of these?

---

**👤 You:**
> "Show my active bookings for the next 7 days."

**🤖 AI Agent:**
> Accessing booking directory... You have 8 appointments scheduled for the upcoming week, including 3 new leads and 5 follow-ups. Shall I retrieve the high-fidelity metadata for the Monday sessions?

---

**👤 You:**
> "Get the transcript for conversation ID '9283'."

**🤖 AI Agent:**
> Fetching transcript... Conversation 9283 was a 4-minute voice call where the customer inquired about pricing and confirmed a booking for Friday. I've retrieved the complete high-fidelity log for you. Need help with the analytics?


## Installation & Usage

To install and use the **AI Receptionist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-receptionist](https://vinkius.com/mcp/ai-receptionist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
