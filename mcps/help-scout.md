# Help Scout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/help-scout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate customer support via Help Scout — manage conversations, customers, and team workflows directly from any AI agent.

## Description
Connect your **Help Scout** help desk to any AI agent and take full control of your customer communication and support operations through natural conversation.

### What you can do

- **Conversation Oversight** — List all active support threads, retrieve full transcripts, and monitor response status.
- **Customer Management** — Access detailed customer profiles and historical interactions to provide personalized service.
- **Team Collaboration** — Add internal notes to conversations and update statuses (active, pending, closed) directly from the chat.
- **Operational Visibility** — List all configured mailboxes, tags, and automated workflows to ensure your help desk is correctly set up.
- **Performance Insights** — Retrieve customer satisfaction ratings to monitor the health of your support operations.
- **Search Capabilities** — Perform advanced searches across your entire conversation history to find answers quickly.

### How it works

1. Subscribe to this server
2. Enter your Help Scout OAuth Access Token
3. Start managing your support operations from Claude, Cursor, or any MCP-compatible client

No more manual exporting of ticket data. Your AI assistant acts as a dedicated Support Coordinator or Customer Success Specialist.

### Who is this for?

- **Support Managers** — instantly retrieve conversation summaries and check agent workloads.
- **Customer Success Teams** — check client history and add internal notes during follow-ups.
- **Operations Leaders** — automate the oversight of mailboxes, tags, and satisfaction ratings.


## Available Tools (12)
- **create_convo_note**: Use this for team collaboration.

Add a private note to a conversation
- **get_conversation**: Get detailed information about a specific conversation
- **get_customer**: Get detailed profile information for a specific customer
- **list_conversations**: Useful for monitoring incoming customer queries.

List support conversations/tickets
- **list_customers**: List all customers registered in the help desk
- **list_mailboxes**: List all configured support mailboxes
- **list_customer_ratings**: List recent customer satisfaction ratings
- **list_tags**: List all available tags for categorizing conversations
- **list_staff_users**: List all support agents/users in the tenant
- **list_workflows**: List automated support workflows
- **search_conversations**: Search for conversations using a query
- **update_convo_status**: Change the status of a conversation (e.g., active, closed)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Help Scout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations in the 'Main' mailbox."

**🤖 AI Agent:**
> I've retrieved your active conversations. You have 5 threads requiring attention, including 'Refund request' from John, 'Feature question' from Maria, and 'API error' from David. Would you like to see the last message for any of these?

---

**👤 You:**
> "Search for conversations from 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching Help Scout... I found 2 conversations for John Doe. One is 'Closed' regarding an old order, and the other is 'Active' regarding a new support query. Should I retrieve the full transcript for the active thread?

---

**👤 You:**
> "Add an internal note to conversation ID 12345: 'Confirmed with engineering, fix arriving tomorrow'."

**🤖 AI Agent:**
> Note added! I've successfully logged your update to conversation 12345. This note is internal-only and will not be seen by the customer. Would you like to set the status to 'Pending' while we wait for the fix?


## ❓ FAQ

**Q: How do I get my Help Scout Access Token?**
You can generate an OAuth2 Access Token by creating an application in the **Help Scout Developer Portal** (developer.helpscout.com). Alternatively, if you are using a personal script, you can use the Client Credentials flow to obtain a token.

**Q: Can I add internal notes to conversations?**
Yes! Use the `create_convo_note` tool. You must provide the `conversation_id` and the text of your note. This allows you to collaborate with your team without the customer seeing the message.

**Q: How do I change the status of a support thread?**
Use the `update_convo_status` tool. Provide the conversation ID and the new status (active, pending, or closed). This helps you keep your mailbox organized.

**Q: Is the integration secure for managing support data?**
Absolutely. The integration uses industry-standard OAuth 2.0 Bearer tokens over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/help-scout](https://vinkius.com/mcp/help-scout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Help Scout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `help-scout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Help Scout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "help-scout": {
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
