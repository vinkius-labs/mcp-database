# Dixa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dixa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage customer conversations, track agents, and monitor support queues via the Dixa API.

## Description
Integrate **Dixa**, the customer friendship platform, directly into your AI workflow. Manage your multi-channel support conversations, monitor agent presence and performance, track service queues, and oversee your support teams using natural language.

### What you can do

- **Conversation Oversight** — List and retrieve detailed information for all customer conversations and their current processing status.
- **Agent Intelligence** — Monitor real-time agent presence, profile details, and team assignments across your organization.
- **Queue Monitoring** — Track active service queues and routing settings to ensure efficient support delivery.
- **Team Management** — List all support teams and identify members assigned to specific organizational units.

### How it works

1. Connect the Dixa integration to your AI assistant.
2. Authorize using your Dixa API Token (found in your organization settings).
3. Orchestrate your customer service and support operations through intuitive conversation.

### Who is this for?

- **Support Managers** — Quickly check queue volumes and agent availability on the go.
- **Customer Success Leads** — Research conversation history and agent performance via chat.
- **Operations Teams** — Monitor support team structures and organizational metadata instantly.


## Available Tools (10)
- **get_service_account_metadata**: Retrieve metadata and usage limits for your Dixa account
- **get_agent_profile**: Get full profile and performance data for a specific agent
- **get_conversation_details**: Get detailed information for a specific customer conversation
- **quick_agent_presence_audit**: Retrieve a high-level summary of active agent presence statuses
- **list_service_agents**: List all support agents registered in your Dixa organization
- **list_customer_conversations**: List all customer service conversations in your Dixa account
- **list_open_support_tickets**: Identify conversations that are currently in an "Open" or "Unassigned" status
- **list_service_queues**: List all active service queues configured in Dixa
- **list_support_teams**: List all configured support teams and their members
- **search_conversations_by_subject**: Search for conversations using a keyword in the subject


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dixa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open support conversations."

**🤖 AI Agent:**
> I've found 8 open conversations, including 'Issues with Payment' and 'Feature Request: Dark Mode'. Would you like to see the assigned agent for any of these?

---

**👤 You:**
> "Show me the details for conversation '12345'."

**🤖 AI Agent:**
> Conversation '12345' (Subject: Login Issue) is currently 'Open' and assigned to 'John Doe'. It was created 2 hours ago via Email. Should I pull the latest message from this conversation?

---

**👤 You:**
> "Who is currently available in the 'Sales' team?"

**🤖 AI Agent:**
> In the Sales team, 3 agents are currently 'Available': 'Alice Johnson', 'Bob Miller', and 'Kenji Tanaka'. 2 other members are 'Away'. Would you like to see the current load for the available agents?


## ❓ FAQ

**Q: How do I get a Dixa API Token?**
Log in to your Dixa account as an administrator, navigate to **Settings > Integrations > API Tokens**, and click **Create Token**. Note that you may need a specific plan for API access.

**Q: Can the agent reply to customers?**
This integration currently focuses on listing and auditing conversations, agents, and queues. Sending replies to customers should be managed via the Dixa agent interface.

**Q: Does the integration show real-time agent presence?**
Yes, you can use the list_service_agents or quick_agent_presence_audit tools to see the current presence status of your support team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dixa](https://vinkius.com/mcp/dixa)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `dixa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dixa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dixa": {
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
