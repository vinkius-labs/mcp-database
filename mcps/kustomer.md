# Kustomer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kustomer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer service — list conversations, audit customers, and search timelines.

## Description
Connect your AI agent to **Kustomer** to streamline your support operations and customer data auditing.

### Key Features

- **Omnichannel Conversation Access** — List and audit support conversations from email, chat, and social channels
- **Customer 360 View** — Fetch detailed customer profiles including custom attributes and history
- **Message Auditing** — Retrieve the full message history for any support interaction
- **Timeline Search** — Perform deep searches across customer timelines using complex JSON filters
- **Service Context** — List support queues, agents, and custom data classes (Klasses)

### Simple Setup

1. Subscribe to this server
2. Log in to Kustomer and generate a **Bearer API Key** (Settings > Security > API Keys)
3. Enter your key in the configuration panel
4. Start managing your support data via natural language


## Available Tools (10)
- **list_kustomer_customers**: Essential for identifying customer IDs for support auditing.

List all customers in Kustomer
- **get_customer_profile**: Get details for a specific customer
- **list_support_conversations**: List recent support conversations
- **get_conversation_details**: Get details for a specific conversation
- **list_conversation_messages**: List all messages in a conversation
- **list_support_queues**: g., Billing, Technical Support) defined in Kustomer.

List active support queues
- **list_kustomer_agents**: List all support agents (users)
- **search_kustomer_timeline**: Provide filters as a JSON string.

Perform a deep search across the customer timeline
- **list_data_klasses**: List Kustomer custom data classes (Klasses)
- **check_kustomer_api_status**: Check the status of the Kustomer API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kustomer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 10 most recent support conversations in Kustomer"

**🤖 AI Agent:**
> I've retrieved the latest 10 conversations. 4 are currently 'Open' and assigned to agents, while 6 are 'Done'. Would you like to audit the messages for the open ones?

---

**👤 You:**
> "Show the full profile for customer '65a4b3c2d1e0f'"

**🤖 AI Agent:**
> Retrieved profile for Jane Doe. She is a 'Platinum' member with a lifetime value of $1,200. Her last contact was via Email 2 days ago regarding a shipping delay.

---

**👤 You:**
> "Search the timeline for customers from 'Brazil'"

**🤖 AI Agent:**
> Searching timeline… I found 15 customers associated with 'Brazil'. 10 have active conversations. Would you like a list of their email addresses?


## ❓ FAQ

**Q: Where do I find my Kustomer API Key?**
Log in to Kustomer, navigate to **Settings** > **Security** > **API Keys**, and create a new key with the necessary scopes.

**Q: Can I see chat messages in real-time?**
The `list_conversation_messages` tool fetches the current history. While not a streaming 'live' view, it provides the most recent state.

**Q: Does this support creating customers?**
The current version focus on data retrieval and analysis. Creation tools are planned for future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kustomer](https://vinkius.com/mcp/kustomer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kustomer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kustomer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kustomer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kustomer": {
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
