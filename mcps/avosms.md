# AvoSMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avosms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Powerful SMS automation — send messages, manage sender IDs, and coordinate contact lists via AI.

## Description
Orchestrate your global mobile communication with **AvoSMS**, the high-performance messaging platform designed for scale. By connecting AvoSMS to your AI agent, you transform SMS outreach from a manual task into a natural conversation. Your agent can now send instant notifications, schedule future broadcasts, manage approved sender identities, and audit your contact lists without you ever touching a dashboard. Whether you're tracking customer responses or monitoring credit balances, your agent acts as a real-time mobile operations manager for your business.

### What you can do

- **Precision Messaging** — Send individual or scheduled SMS messages globally with full support for custom delivery timestamps.
- **Identity Control** — Request, list, and manage approved Sender IDs (names) to ensure your brand is always recognized.
- **Contact Orchestration** — Create and manage dedicated contact lists, adding recipients dynamically via natural language.
- **Response Auditing** — Retrieve and list incoming SMS responses to maintain a two-way dialogue with your audience.
- **Account Health** — Instantly check your remaining credit balance and verify account connectivity on the fly.

### How it works

1. Subscribe to this server
2. Enter your AvoSMS Account ID and API Key
3. Start communicating with your customers via SMS through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — automate campaign delivery and manage opt-in contact lists through natural language.
- **Customer Support** — send instant alerts and read incoming customer responses directly from your chat interface.
- **Operations Leads** — monitor SMS credit consumption and verify delivery health across global networks.
- **Developers** — integrate reliable SMS capabilities into AI workflows for verification or notifications.


## Available Tools (11)
- **add_contact**: Add a contact to a list
- **create_list**: Create a new contact list
- **create_sender**: Request a new sender ID
- **delete_list**: Delete a contact list
- **delete_sender**: Delete a sender ID
- **get_account_check**: Verify AvoSMS account connection
- **get_balance**: Check remaining SMS credits balance
- **list_responses**: List incoming SMS responses
- **list_lists**: List all contact lists
- **list_senders**: List all approved sender IDs
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AvoSMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +33600000000 saying 'Your order is ready for pickup!' using sender 'ShopAlert'."

**🤖 AI Agent:**
> I've sent the SMS to +33600000000. It will appear on the recipient's phone as 'ShopAlert'.

---

**👤 You:**
> "Check my AvoSMS credit balance and list recent replies."

**🤖 AI Agent:**
> Your current balance is 450.5 credits. I also found 3 recent responses from customers. Would you like me to read them for you?

---

**👤 You:**
> "Add the phone number +123456789 to my 'VIP Customers' list."

**🤖 AI Agent:**
> I've added +123456789 to the 'VIP Customers' list (ID: 9876). Your list is now updated and ready for future campaigns.


## ❓ FAQ

**Q: What is a sender ID and why do I need one?**
A sender ID is the alphanumeric label (3-11 characters) that appears as the sender on the recipient's phone. Approved sender IDs help increase trust and open rates for your messages.

**Q: Can I receive replies to my SMS messages?**
Yes! Use the `list_responses` tool to retrieve any incoming messages from your customers. This allows your agent to handle two-way communication workflows.

**Q: How do I ensure my SMS is delivered at a specific time?**
When using the `send_sms` tool, provide a YYYY-MM-DD HH:MM:SS string in the `date` parameter. AvoSMS will queue the message and deliver it exactly at the requested time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avosms](https://vinkius.com/mcp/avosms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AvoSMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `avosms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AvoSMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "avosms": {
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
