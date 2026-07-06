# HelpCrunch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpcrunch-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Engage customers with live chat, email automation, and a knowledge base that reduces support workload and boosts satisfaction.

## Description
Connect your **HelpCrunch** account to any AI agent and take full control of your customer support and multi-channel communication workflows through natural conversation.

### What you can do

- **Unified Chat Management** — List and manage all customer conversations and retrieve detailed chat metadata and history
- **Proactive CRM** — Create and update customer profiles programmatically to maintain a high-fidelity database of user attributes and activities
- **Real-time Messaging** — Send and receive messages within chats directly through your agent to provide instant customer assistance
- **Support Orchestration** — Update chat statuses (open, pending, closed) and monitor department workloads for efficient team routing
- **Agent Visibility** — Retrieve team agent directories and status to understand support capacity across your organization

### How it works

1. Subscribe to this server
2. Retrieve your API Key from your HelpCrunch dashboard (Settings > Developers > Public API)
3. Start managing your customer communications from Claude, Cursor, or any MCP client

No more manual toggling between chat windows or searching for customer emails. Your AI acts as your dedicated support coordinator.

### Who is this for?

- **Support Teams** — instantly triage chat queues and respond to high-priority queries using natural language
- **Customer Success Managers** — update user attributes and retrieve interaction history without leaving your workspace
- **Sales Representatives** — identify and manage new leads from live chat interactions through automated queries


## Available Tools (12)
- **get_customer_details**: Get details for a specific customer
- **list_team_agents**: List all agents/team members
- **list_conversations**: List all customer chats
- **list_customers**: List all customers
- **list_departments**: List all departments
- **list_messages_in_chat**: List messages from a specific chat
- **list_active_webhooks**: List configured webhooks
- **search_customers**: Search for customers using filters
- **send_chat_message**: Can be sent as an agent.

Post a message to a chat
- **update_conversation_status**: g., open, pending, closed).

Change chat status
- **create_customer**: Requires email and name.

Create a new customer profile
- **get_conversation_details**: Get details for a specific chat


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HelpCrunch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customer chats in HelpCrunch."

**🤖 AI Agent:**
> I've found 5 active conversations. Notable chats include an inquiry from 'John' (ID: c_101) about pricing and a support request from 'Sarah' (ID: c_102). Which one should I open for you?

---

**👤 You:**
> "Search for customer with email 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've located Jane Doe's profile (ID: 789). She is a 'VIP' customer based in London and has 3 previous interactions with our support team. Would you like to see her full activity history?

---

**👤 You:**
> "Send a message to chat ID 'c_101' saying 'I'm checking that for you right now'."

**🤖 AI Agent:**
> Done! Message delivered to chat c_101. The customer will see your reply in the chat window immediately. I'll let you know if they respond.


## ❓ FAQ

**Q: How do I generate an API Key in HelpCrunch?**
Log in to your HelpCrunch account, navigate to **Settings** > **Developers** > **Public API**, and click **Generate New API Key** to obtain your token.

**Q: Can the agent respond to customers directly?**
Yes! Use the `send_chat_message` tool to post replies into any active chat thread. The message will appear as coming from your agent account.

**Q: How do I search for a customer by email?**
The `search_customers` tool allows you to perform lookups using filters like email, name, or external ID to retrieve specific user profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpcrunch-alternative](https://vinkius.com/mcp/helpcrunch-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HelpCrunch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `helpcrunch-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HelpCrunch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "helpcrunch-alternative": {
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
