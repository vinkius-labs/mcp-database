# AgentMail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agentmail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Give your AI agents their own email inbox to read, send, and reply to messages natively.

## Description
Connect **AgentMail** to your AI agent and unlock a programmable email client. Stop relying on complex integrations and grant your agent its own functional inbox to communicate with the world.

### What you can do

- **Inboxes** — Create, list, and delete custom email addresses on the fly for your agent
- **Threads** — Scan active conversations and read full historical threads natively
- **Messages** — Send new emails, reply contextually to specific threads, and forward messages
- **Attachments** — Extract and process files attached to incoming emails automatically

### How it works

1. Subscribe to this server
2. Enter your AgentMail API Key
3. Start managing emails from Claude, Cursor, or any MCP-compatible client

Give your AI the ability to reach out, follow up, and monitor replies autonomously.

### Who is this for?

- **AI Developers** — build autonomous agents that communicate with users via email
- **Customer Support** — deploy agents that read incoming tickets and draft thoughtful replies
- **Sales Automation** — let your agent handle outreach and monitor responses automatically


## Available Tools
- **list_inboxes**: An inbox is required to send or receive emails. Returns an array of inboxes with their IDs, email addresses, and names.

List all inboxes assigned to the AgentMail API Key
- **get_inbox**: Get details of a specific inbox by ID
- **create_inbox**: You can optionally link it to a custom domain.

Create a new email inbox for an agent
- **delete_inbox**: Warning: this deletes all emails in it.

Delete a specific inbox by ID
- **list_threads**: Returns a list of thread objects including subject lines and recent message previews. The agent needs an inbox_id first.

List conversation threads inside an inbox
- **get_thread**: Requires a thread_id.

Read all messages inside a specific conversation thread
- **get_attachment**: Attachments might be encoded in base64. Ensure you parse or read it correctly.

Download or read a specific attachment from a message
- **send_message**: Requires the sender inbox_id, which you can get from list_inboxes.

Send a brand new email message
- **reply_to_message**: The thread will be preserved.

Reply to an existing email message/thread
- **forward_message**: You can optionally add text to the forwarded message.

Forward an existing email message
- **update_message**: Update an existing message metadata (like marking it as read)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AgentMail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new inbox for our support team."

**🤖 AI Agent:**
> I have created a new inbox with the address support-agent-123@agentmail.to. It is now active and ready to receive messages. Would you like me to configure an automated welcome reply?

---

**👤 You:**
> "Check all my unread threads in the main inbox today."

**🤖 AI Agent:**
> You have 2 unread threads. The first is an inquiry from a prospective client asking for pricing details. The second is a generic marketing email. Would you like me to draft a contextual reply for the client?

---

**👤 You:**
> "Reply to the client thanking them and attach the pricing PDF."

**🤖 AI Agent:**
> The email has been successfully sent. I replied directly to the client's thread, thanked them for their interest, and included the 'Pricing_2024.pdf' attachment as requested.


## ❓ FAQ

**Q: Does my AI agent need a preexisting Gmail or Outlook account to use this?**
No. AgentMail is entirely standalone. You can use your agent to programmatically provision brand new, unique email addresses in seconds, completely independent of legacy email providers.

**Q: Can my agent download files that users send to its email address?**
Yes. When scanning threads in the inbox, your agent will detect any attached files. It can then use the dedicated attachments tool to retrieve and analyze the contents of the file before drafting a reply.

**Q: Is it possible to manage multiple outreach campaigns at the same time?**
Absolutely. Your agent can create and manage multiple inboxes simultaneously. It can list all active boxes, read unread threads for each, and contextualize its replies based on the specific campaign inbox.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agentmail](https://vinkius.com/mcp/agentmail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AgentMail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `agentmail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AgentMail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agentmail": {
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
