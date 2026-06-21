# Mailosaur MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailosaur)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate email and SMS testing and management via the Mailosaur REST API.

## Description
Connect your **Mailosaur** account to any AI agent to automate your email and SMS testing workflows. This MCP server enables your agent to manage virtual servers (inboxes), retrieve and search for messages, and extract content for validation directly from natural language interfaces.

### What you can do

- **Virtual Inbox Oversight** — List and manage all virtual servers and retrieve their unique routing domains
- **Message Retrieval** — List all email and SMS messages received by a specific server instantly
- **Advanced Search** — Find specific messages by sender, recipient, subject, or body content using detailed criteria
- **Content Inspection** — Retrieve the full HTML and text content of any message for automated validation
- **Inbox Maintenance** — Clear entire server inboxes or delete specific messages via simple commands
- **Dynamic Infrastructure** — Create and configure new virtual servers programmatically for testing isolation

### How it works

1. Subscribe to this server
2. Enter your Mailosaur API Key
3. Start managing your test communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the verification of transactional emails and SMS codes via natural language commands
- **Developers** — Quickly inspect incoming test emails and clear virtual inboxes directly from your IDE
- **Operations Teams** — Monitor automated communication flows and audit incoming messages effortlessly


## Available Tools
- **create_virtual_server**: Create a new virtual server/inbox
- **clear_server_inbox**: Delete all messages in a server
- **delete_specific_message**: Permanently remove a message
- **get_message_content**: Get the full content of a specific message
- **get_server_details**: Get details for a specific virtual server
- **list_server_messages**: List all messages in a virtual server
- **search_server_messages**: Requires a server ID and criteria like sentTo, sentFrom, or subject.

Search for specific messages using criteria
- **list_virtual_servers**: Use this to identify server IDs.

List all Mailosaur virtual servers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailosaur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Mailosaur servers."

**🤖 AI Agent:**
> I've retrieved your servers. You have 3 active environments: 'Production Tests (ID: prod123)', 'Staging Inboxes', and 'Dev Sandbox'.

---

**👤 You:**
> "Find the last message sent to 'test-user@mailosaur.io' in server 'prod123'."

**🤖 AI Agent:**
> I've searched server prod123. I found 1 message sent to test-user@mailosaur.io with the subject 'Welcome to our Service'. Would you like to see the full content?

---

**👤 You:**
> "Delete all messages in the 'Dev Sandbox' server (ID: 'dev789')."

**🤖 AI Agent:**
> I've successfully cleared the inbox for server dev789. All messages have been permanently removed.


## ❓ FAQ

**Q: How do I find my Server ID?**
Use the `list_virtual_servers` tool to see a comprehensive list of all servers in your account along with their unique IDs.

**Q: Can I search for messages by recipient email?**
Yes, use the `search_server_messages` tool and provide a JSON criteria object with the `sentTo` field.

**Q: Does Mailosaur support SMS messages?**
Absolutely. Mailosaur treats SMS messages similarly to emails. You can list and search for them within your virtual servers just like email content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailosaur](https://vinkius.com/mcp/mailosaur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailosaur** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mailosaur` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailosaur** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailosaur": {
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
