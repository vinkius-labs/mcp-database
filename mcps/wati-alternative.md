# Wati MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wati-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send WhatsApp messages at scale with official API access, chatbot automation, and shared team inbox for business conversations.

## Description
Connect your **Wati** WhatsApp Business account to any AI agent and simplify how you engage with your customers through natural conversation and automated messaging workflows.

### What you can do

- **Direct Messaging** — Send instant WhatsApp session messages to active contacts for real-time support and engagement.
- **Template Automation** — Send pre-approved WhatsApp templates to start conversations or send notifications with dynamic parameters.
- **Contact Management** — List and inspect your WhatsApp subscribers and contacts to keep your directory up-to-date.
- **Chat History** — Retrieve the complete message history for any specific contact to understand the conversation context.
- **Template Catalog** — List all available message templates to identify the best options for your communication strategy.

### How it works

1. Subscribe to this server
2. Enter your Wati API Key and API Endpoint (found in your Wati API dashboard)
3. Start managing your WhatsApp communication from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support Teams** — quickly respond to inquiries and retrieve chat history via simple AI commands.
- **Sales & Marketing** — automate the sending of template-based notifications and manage lead contacts directly.
- **Operations Managers** — monitor communication flows and verify template availability without leaving the workspace.


## Available Tools (13)
- **get_template**: Get template details
- **list_templates**: List message templates
- **list_broadcasts**: List broadcasts
- **list_contacts**: List contacts
- **list_messages**: List messages
- **list_tags**: List tags
- **send_media_message**: Send media message
- **send_session_message**: Send a session message
- **send_template_message**: Send a template message
- **update_contact**: Update contact attributes
- **add_contact**: Add a contact
- **check_wati_status**: Verify connectivity
- **get_contact**: Get contact details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wati** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my WhatsApp templates."

**🤖 AI Agent:**
> I've retrieved your message templates. You have 5 approved templates including 'Welcome Message', 'Order Confirmation', and 'Shipping Update'. Which one would you like to use?

---

**👤 You:**
> "Send the 'order_ready' template to 5511999999999."

**🤖 AI Agent:**
> Template message sent! I've triggered the 'order_ready' template to the recipient 5511999999999. The message ID is WATI_8823.

---

**👤 You:**
> "Show me the chat history for the number 5511888888888."

**🤖 AI Agent:**
> I've fetched the history. The last 3 messages show the customer asking about pricing, followed by your response and a confirmation of payment. Would you like to see the full transcript?


## ❓ FAQ

**Q: What is the difference between a session message and a template message?**
Session messages can only be sent if the user has messaged you in the last 24 hours. Template messages are pre-approved by WhatsApp and can be used to initiate a conversation at any time.

**Q: How do I see the approved templates in my account?**
Use the `list_message_templates` query. Your agent will retrieve the complete list of pre-approved WhatsApp templates available in your Wati dashboard.

**Q: Can I retrieve the last messages from a specific customer?**
Yes! Use the `list_chat_history` tool and provide the customer's WhatsApp number. The agent will return the message history for that specific conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wati-alternative](https://vinkius.com/mcp/wati-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wati** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wati-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wati** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wati-alternative": {
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
