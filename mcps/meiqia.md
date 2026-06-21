# MeiQia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meiqia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Leading live chat and customer CRM platform — manage conversations, messages, and customers via AI.

## Description
Empower your AI agent to orchestrate your customer engagement with **MeiQia** (美洽), the premier live chat and CRM platform for modern businesses. By connecting MeiQia to your agent, you transform complex conversation tracking and customer relationship management into a natural conversation. Your agent can instantly list active chats, retrieve full message histories, update customer profiles, and even monitor agent workloads without you needing to navigate the web interface. Whether you are managing real-time sales queries or resolving support issues, your agent acts as a real-time engagement assistant, keeping your data accurate and your communication responsive.

### What you can do

- **Conversation Orchestration** — List all active and closed conversations across your MeiQia workspace.
- **Message Management** — Retrieve full message histories and send agent responses directly through the chat interface.
- **Customer CRM Control** — Browse and manage customer profiles, including contact details and interaction history.
- **Agent Coordination** — Monitor support agents and retrieve their real-time online status.
- **Performance Insights** — Retrieve high-level summaries of team workload and engagement statistics.

### How it works

1. Subscribe to this server
2. Enter your MeiQia Access Token
3. Start managing your customer engagement through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — track engagement quality, audit conversations, and monitor team responsiveness through natural language.
- **Support Agents** — manage multiple customer chats and update CRM profiles directly from your AI-powered workspace.
- **Sales Operations** — coordinate leads and monitor real-time sales queries via a unified AI interface.
- **Business Owners** — get real-time insights into organization-wide customer engagement and agent performance.


## Available Tools
- **create_customer**: Create a new customer
- **get_agent_status**: Get agent online status
- **get_conversation**: Get conversation details
- **get_customer**: Get customer details
- **get_workload_summary**: Get team workload summary
- **list_agents**: List support agents
- **list_conversations**: List live chat conversations
- **list_customers**: List CRM customers
- **list_messages**: List conversation messages
- **send_message**: Send message to customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeiQia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open conversations on MeiQia."

**🤖 AI Agent:**
> I've retrieved your open conversations. There are 8 active chats, including queries about 'API integration' and 'Enterprise pricing'. Which one would you like to view messages for?

---

**👤 You:**
> "Send a reply to conversation 'conv-8821' saying 'We are looking into this for you'."

**🤖 AI Agent:**
> Done! I've sent your reply to the customer in conversation 'conv-8821'. Your message 'We are looking into this for you' has been successfully delivered.

---

**👤 You:**
> "Show me the profile for customer 'Mario'."

**🤖 AI Agent:**
> I've retrieved the profile for Mario. He is a high-value customer from 'Tech Corp' with a history of 12 interactions. Would you like me to list his recent messages or update his contact info?


## ❓ FAQ

**Q: How do I obtain a MeiQia Access Token?**
Log in to your MeiQia workspace, go to [Settings] → [Developer] → [APIs], and generate a new Access Token. Make sure to copy it carefully.

**Q: Can I reply to customers through the agent?**
Yes. Use the `send_message` tool with the specific conversation ID and your message content. This allows for rapid responses directly from your AI workspace.

**Q: Is it possible to see the current team workload?**
Yes! Use the `get_workload_summary` tool to retrieve a real-time overview of how many active chats each agent is handling, helping you manage team capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meiqia](https://vinkius.com/mcp/meiqia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MeiQia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meiqia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MeiQia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meiqia": {
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
