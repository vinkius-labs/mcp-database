# Dixa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dixa-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Route customer conversations to the right agent across phone, email, chat, and messaging with intelligent prioritization.

## Description
Connect your **Dixa** account to any AI agent and take full control of your omnichannel customer service and team coordination workflows through natural conversation.

### What you can do

- **Conversation Orchestration** — List and manage active support tickets programmatically, including retrieving detailed metadata and historical context
- **Agent & Team Coordination** — Assign conversations to yourself or specific team members and monitor agent availability in real-time to optimize response times
- **Customer Profile Intelligence** — Access and manage end-user (customer) profiles programmatically to maintain a high-fidelity record of contact information and interaction history
- **Lifecycle Management** — Programmatically create new support requests or mark existing conversations as resolved/closed to maintain a structured support pipeline
- **Operational Monitoring** — Check API connectivity and monitor active webhooks directly through your agent for reliable service operations

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from the Dixa dashboard (Settings > Integrations > API Tokens)
3. Start managing your customer interactions from Claude, Cursor, or any MCP client

No more manual ticket shuffling or digging through agent lists in the portal. Your AI acts as your dedicated support strategist and CX coordinator.

### Who is this for?

- **Support Leads & Managers** — instantly retrieve ticket summaries and reassign high-priority conversations using natural language commands
- **Customer Success Teams** — monitor customer profiles and interaction history without leaving your communication tools
- **Operations Leads** — verify system health and manage webhook configurations through simple AI queries


## Available Tools (12)
- **create_customer_profile**: Add new customer
- **get_connection_status**: Check API health
- **get_agent_info**: Get agent details
- **get_conversation_details**: Get ticket info
- **list_support_agents**: List active agents
- **list_conversations**: List customer tickets
- **list_support_teams**: List agent teams
- **list_end_users**: List Dixa customers
- **list_active_webhooks**: Get event configs
- **assign_to_self**: Claim a conversation
- **resolve_conversation**: Close a conversation
- **create_conversation**: Add new support chat


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dixa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations in Dixa."

**🤖 AI Agent:**
> I've retrieved your active conversations. You currently have 4 tickets needing attention, including 'Refund Request' (ID: conv_1) and 'Login Issue'. Which one would you like to reassign or resolve?

---

**👤 You:**
> "Find the customer profile for 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've located Jane Doe's profile (ID: usr_123). She has a history of 3 past conversations and is currently assigned to the 'VIP' queue. Shall I retrieve her full interaction history?

---

**👤 You:**
> "Mark conversation ID 'conv_456' as resolved."

**🤖 AI Agent:**
> Action complete! Conversation conv_456 has been successfully marked as resolved in Dixa. The status is now updated on your dashboard. Need help with any other tickets?


## ❓ FAQ

**Q: How do I find my Dixa API Token?**
Log in to Dixa, navigate to **Settings** > **Integrations** > **API Tokens**, and generate a new token for your integration.

**Q: Can I assign tickets to myself via AI?**
Yes! Use the `assign_to_self` tool with a specific conversation ID to take ownership of a support ticket.

**Q: How do I check which agents are online?**
The `list_support_agents` tool retrieves all agent profiles and their current status directly from the Dixa platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dixa-alternative](https://vinkius.com/mcp/dixa-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dixa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dixa-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dixa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dixa-alternative": {
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
