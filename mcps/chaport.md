# Chaport MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chaport)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage live chat and customer messaging via Chaport — track visitors, send messages, and monitor operator status directly from any AI agent.

## Description
Connect your **Chaport** account to any AI agent and take full control of your customer messaging operations through natural conversation. Streamline how you engage with website visitors and manage your support team.

### What you can do

- **Live Messaging** — Send and receive messages in active chat sessions natively
- **Visitor Intelligence** — List and retrieve details for recent website visitors and their contact info flawlessly
- **Conversation History** — Access full chat histories and event logs to understand customer context securely
- **Operator Oversight** — Monitor agent availability and list all operators in your account in real-time
- **Status Management** — Identify which agents are currently online to manage support load flawlessly
- **Agent Insights** — Retrieve your own operator profile and account metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chaport API Token (obtained from Settings -> API)
3. Start managing your customer chats from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor agent status and review chat histories using natural language
- **Customer Success Teams** — identify recent visitors and engage with them without opening the dashboard
- **Sales Reps** — quickly look up visitor details and previous interactions straight from their chat interface
- **Business Owners** — audit support team activity and customer engagement levels


## Available Tools (8)
- **get_chat_history**: Retrieve the message history and events for a specific chat
- **get_my_agent_profile**: Retrieve information about the authenticated agent
- **get_visitor_last_chat**: Retrieve the last chat session for a specific visitor
- **get_visitor_details**: Get detailed information for a specific visitor
- **list_online_agents**: List all agents who are currently online
- **list_chaport_operators**: List all operators in your Chaport account
- **list_website_visitors**: List recent visitors to your website
- **send_agent_message**: Send a message to a visitor in a specific chat


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chaport** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all website visitors from the last hour."

**🤖 AI Agent:**
> Retrieving recent visitors... I found 5 visitors, including 'John Doe' (john@example.com) and 4 anonymous guests. Would you like to see the details for any of them?

---

**👤 You:**
> "Which support agents are currently online in Chaport?"

**🤖 AI Agent:**
> Checking agent status... Currently, 2 operators are online: Sarah Miller and Mike Scott. The other 3 agents are currently offline.

---

**👤 You:**
> "Show me the message history for chat ID 123456."

**🤖 AI Agent:**
> Retrieving history for chat 123456... I found 10 events, including 4 messages from the visitor and 3 replies from Sarah Miller. Would you like to see the transcript?


## ❓ FAQ

**Q: Can I see who is currently visiting my website?**
Yes! Use the `list_website_visitors` tool. The agent will return a list of recent and active visitors, including their names, emails, and location if available.

**Q: How do I reply to a specific customer chat?**
Use the `send_agent_message` tool with the unique chat ID. Your agent will post the message directly into the Chaport conversation.

**Q: Where do I generate my Chaport API Token?**
Log in to your Chaport account and go to **Settings → API**. You can generate and copy your API token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chaport](https://vinkius.com/mcp/chaport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chaport** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chaport` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chaport** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chaport": {
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
