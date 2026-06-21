# Sobot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sobot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Leading AI customer support and ticketing platform in China — manage tickets, agents, and knowledge via AI.

## Description
Empower your AI agent to orchestrate your customer service with **Sobot** (智齿科技), the premier AI-driven customer support platform in China. By connecting Sobot to your agent, you transform complex ticketing management and agent coordination into a natural conversation. Your agent can instantly list your work orders, retrieve agent statuses, browse knowledge base articles, and even audit chat histories without you ever needing to navigate the comprehensive web interface. Whether you are managing a high-volume support team or a specific high-priority ticket, your agent acts as a real-time support operations assistant, keeping your data accurate and your customers satisfied.

### What you can do

- **Ticket Management** — List all active work orders, get detailed information, and create new tickets instantly.
- **Agent Coordination** — Browse support agents and monitor their real-time online/busy status.
- **Knowledge Retrieval** — List and retrieve content from your Sobot knowledge base to assist with customer queries.
- **Chat Audit** — Browse historical chat records and transcripts to track customer engagement.
- **Service Insights** — Retrieve high-level summaries of organization-wide support activity and performance.

### How it works

1. Subscribe to this server
2. Enter your Sobot App ID and App Key
3. Start managing your customer support through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Managers** — track team performance, audit ticket statuses, and monitor agent availability through natural language.
- **Support Engineers** — manage your assigned tickets and retrieve knowledge articles directly from your AI-powered workspace.
- **Operations Teams** — oversee service quality and monitor activity summaries across multiple support channels.
- **Sobot Power Users** — integrate your existing support workflows into your AI-driven daily routines.


## Available Tools (10)
- **create_ticket**: Create a new ticket
- **get_agent_status**: Get agent online status
- **get_knowledge_detail**: Get knowledge article details
- **get_org_summary**: Get organization activity summary
- **get_ticket_details**: Get ticket details
- **list_agents**: List support agents
- **list_chat_history**: List chat history
- **list_knowledge**: List knowledge base articles
- **list_tickets**: List customer support tickets
- **list_users**: List customers/users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sobot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active support tickets from Sobot."

**🤖 AI Agent:**
> I've retrieved your active Sobot tickets. You have 15 pending tickets, including 'Login issue' and 'Refund request'. Would you like more details on any of them?

---

**👤 You:**
> "Check if agent 'Mario' is currently online."

**🤖 AI Agent:**
> I've checked the status for agent Mario. He is currently 'Online' and ready to take new chats. Would you like me to assign a ticket to him?

---

**👤 You:**
> "Search the knowledge base for 'refund policy'."

**🤖 AI Agent:**
> I've found an article titled 'Refund Policy and Procedures' in your Sobot knowledge base. It details the steps for processing refunds and the eligibility criteria. Shall I retrieve the full content for you?


## ❓ FAQ

**Q: How do I obtain my Sobot App ID and Key?**
You need to contact your Sobot business manager or support personnel to apply for your unique `appid` and `app_key`.

**Q: Can I check if an agent is currently online?**
Yes. Use the `get_agent_status` tool with the specific agent ID to retrieve their real-time status, including whether they are online, busy, or offline.

**Q: Is it possible to retrieve knowledge base articles through the agent?**
Yes! You can list available articles using `list_knowledge` and retrieve the full content of a specific document using the `get_knowledge_detail` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sobot](https://vinkius.com/mcp/sobot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sobot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sobot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sobot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sobot": {
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
