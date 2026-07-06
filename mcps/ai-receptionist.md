# AI Receptionist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-receptionist)
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


## Available Tools (10)
- **get_aireceptionist_booking**: Get booking details
- **get_aireceptionist_conversation**: Get conversation details
- **get_aireceptionist_me**: Get current user profile
- **list_aireceptionist_bookings**: List active bookings
- **list_aireceptionist_conversations**: List AI conversations
- **list_aireceptionist_knowledge**: List knowledge base articles
- **list_aireceptionist_webhooks**: List active webhooks
- **create_aireceptionist_booking**: Create a booking
- **create_aireceptionist_conversation**: Create a new conversation
- **get_aireceptionist_analytics**: Get performance analytics


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


## ❓ FAQ

**Q: How do I find my AI Receptionist API Key?**
Log in to your account, navigate to **Developer Settings** > **API**, and generate or copy your unique API Key.

**Q: Can I read call transcripts via AI?**
Yes! The `get_aireceptionist_conversation` tool allows your agent to retrieve complete high-fidelity transcripts of any AI interaction programmatically.

**Q: How do I check lead analytics?**
Use the `get_aireceptionist_analytics` tool to retrieve a high-fidelity summary of lead capture metrics and performance data directly through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-receptionist](https://vinkius.com/mcp/ai-receptionist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Receptionist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-receptionist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Receptionist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-receptionist": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
