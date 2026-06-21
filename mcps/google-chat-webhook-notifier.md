# Google Chat Webhook Notifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-chat-webhook-notifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it sends messages to your Google Chat spaces. That's its only function, and nothing else. Incredible for giving your AI agents a voice.

## Description
We refused to build a bloated Google Workspace integration that demands terrifying OAuth scopes across your entire corporate domain via the Google Chat API. Instead, this MCP server provides a surgical, zero-trust bridge: **a single Incoming Webhook URL.**

Your AI agent gains the immediate, zero-friction ability to drop critical alerts, deployment statuses, and rich engineering reports straight into the designated Google Chat space without compromising your organization's security.

### The Superpowers

- **Zero-Bloat Deployment:** No heavy Google Cloud Projects to configure, no service accounts to manage. If you can generate a webhook, your AI can speak.
- **Native Cards v2 Mastery:** The agent isn't limited to boring plain text. It can programmatically generate rich Cards v2 layouts—complete with interactive buttons, styled text, and structured data grids.
- **Absolute Containment:** Because it's just a webhook, the agent cannot read your corporate emails, cannot snoop on other Google Chat spaces, and cannot cause chaos. It is the purest, safest way to give your AI a megaphone in the Google Workspace world.


## Available Tools
- **send_google_chat_message**: Provide the fallback text in the "text" parameter. Optionally, provide a rich UI element via the "cardJson" string.

Send a notification or message to a Google Chat Space via Webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Chat Webhook Notifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Notify Google Chat that the database backup is finished."

**🤖 AI Agent:**
> I've sent the message 'The database backup is finished.' to the Google Chat space.

---

**👤 You:**
> "Send a rich alert to Google Chat using a Cards v2 layout for a security incident."

**🤖 AI Agent:**
> The rich Cards v2 alert detailing the security incident has been successfully posted to Google Chat.


## ❓ FAQ

**Q: Can the agent read messages from Google Chat with this?**
No. Google Chat Incoming Webhooks are strictly unidirectional (Push only). The agent can only *send* messages to the authorized space. It cannot read the space history or see replies. This ensures absolute Zero-Trust containment.

**Q: How do I create a Google Chat Webhook URL?**
In Google Chat, go to the space, click the space name dropdown, select 'Apps & integrations', click 'Manage webhooks', and add one. Name your webhook and copy the generated URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-chat-webhook-notifier](https://vinkius.com/mcp/google-chat-webhook-notifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Chat Webhook Notifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-chat-webhook-notifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Chat Webhook Notifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-chat-webhook-notifier": {
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
