# WhatsApp Message Sender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-message-sender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it sends text messages using the official Meta WhatsApp Cloud API. That's its only function, and nothing else. Incredible for giving your AI agents direct access to customers.

## Description
We refused to build a complex conversational chatbot system that forces you into a specific workflow. Instead, this MCP server provides a surgical, zero-trust bridge: **just sending text messages via WhatsApp.**

Your AI agent gains the immediate, zero-friction ability to drop status updates, payment confirmations, or emergency alerts straight to any WhatsApp user, bridging the gap between your systems and the most popular messaging app in the world.

### The Superpowers

- **Direct Customer Reach:** When an agent finishes a task (like processing an order or analyzing a report), it can immediately ping the user directly on WhatsApp.
- **Zero-Bloat Integration:** No massive SDKs. It uses the direct REST API endpoint (`/messages`). You only need your Meta Phone Number ID and Access Token.
- **Absolute Containment:** Because this is strictly a sending tool using the official Meta Cloud API, the agent cannot read your WhatsApp inbox, cannot snoop on replies, and cannot alter your Business Manager settings. It is a secure, pure one-way megaphone.


## Available Tools
- **send_whatsapp_message**: Provide the destination phone number in E.164 format WITHOUT the plus sign (e.g., 5511999999999 for Brazil) in the "to" parameter, and the text in the "body" parameter. Note: Sending to users outside of the 24-hour service window requires pre-approved templates on the Meta API, otherwise it may fail.

Send a text message directly to a WhatsApp number using the Meta Cloud API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhatsApp Message Sender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to 5511999999999 saying that their order is out for delivery."

**🤖 AI Agent:**
> I've successfully dispatched the WhatsApp message.


## ❓ FAQ

**Q: Can the agent read incoming WhatsApp replies with this?**
No. This MCP utilizes the REST API strictly for creating new messages. It does not configure or expose incoming webhooks, meaning it acts strictly as a one-way notification megaphone. It cannot see your customer's replies.

**Q: Why are some messages failing to send?**
The Meta WhatsApp Cloud API has a strict 24-hour service window. If you are sending a free-form text message to a user who hasn't messaged you in the last 24 hours, the API will block it unless you use a pre-approved Message Template. Ensure you are within the 24-hour window for free-form replies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-message-sender](https://vinkius.com/mcp/whatsapp-message-sender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WhatsApp Message Sender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `whatsapp-message-sender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WhatsApp Message Sender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whatsapp-message-sender": {
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
