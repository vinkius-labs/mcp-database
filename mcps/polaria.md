# Polaria MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polaria)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Unify your customer support with an AI agent that manages Polaria conversations, contacts, and FAQ retrieval.

## Description
Transform your customer support operations by connecting Polaria directly to your AI agent. Let your assistant automatically retrieve relevant help articles, instantly respond to customer conversations, and efficiently manage your user directory without navigating away from your central workspace.

### What you can do
- Access and organize your entire customer contact database
- Read and respond to live chat conversations instantly
- Update the status of support tickets (Open, Pending, Resolved)
- Retrieve FAQ articles to resolve customer inquiries faster
- Manage custom attributes for targeted support

### How it works
1. Log into your Polaria dashboard
2. Create a new app under Settings > Marketplace to get your Secret Key
3. Connect via Vinkius to unleash AI-powered conversational support

### Who is it for?
Ideal for customer success teams, support agents, and community managers who want to resolve user queries faster and automate repetitive chat tasks.


## Available Tools (8)
- **create_contact**: Create a new contact in Polaria
- **add_chat_message**: Add a message to a conversation
- **get_contact**: Get details of a specific contact
- **get_conversation**: Get details of a specific conversation
- **list_contacts**: List contacts in Polaria
- **list_conversations**: List conversations in Polaria
- **list_faqs**: List FAQs in Polaria
- **list_widgets**: List Polaria widgets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polaria** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in Polaria."

**🤖 AI Agent:**
> You have 1,240 contacts in Polaria. Would you like me to filter them by a specific segment or recent activity?

---

**👤 You:**
> "Show recent chat conversations."

**🤖 AI Agent:**
> Here are the 3 most recent chat conversations: 1) Billing issue with John Doe (Open), 2) Refund request from Acme Corp (Pending), 3) Technical support for Sarah (Resolved).

---

**👤 You:**
> "Add a reply message to conversation 'C123'."

**🤖 AI Agent:**
> I've successfully added your reply to conversation 'C123' and marked the status as 'Waiting on Customer'.


## ❓ FAQ

**Q: Where do I find my Secret Key?**
Log in to Polaria, go to Settings > Marketplace > Create my own app, create a new application, and show the 'Secret Key' in the authorized applications section.

**Q: What is the Base URL for the API?**
The Polaria REST API v2 base URL is: https://polaria.ai/rest/v2/

**Q: Can I modify existing conversations?**
Yes, you can add replies and change the status of existing conversations directly using the Polaria MCP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polaria](https://vinkius.com/mcp/polaria)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polaria** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polaria` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polaria** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polaria": {
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
