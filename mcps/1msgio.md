# 1msg.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/1msgio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Official WhatsApp Business API automation — send messages, manage templates, and monitor channel status via AI.

## Description
Transform your **1msg.io** instance into a conversational powerhouse for your AI agent. This integration bridges the gap between the official WhatsApp Business API and your AI workflows, allowing you to handle customer engagement, notifications, and channel health directly through natural language. Whether you are automating support or orchestrating marketing broadcasts, your agent acts as a direct bridge to your WhatsApp audience, ensuring every interaction follows official Meta standards.

### What you can do

- **Official Messaging** — Send text and media messages (images, PDF, video) to any WhatsApp number worldwide using official API standards
- **Template Management** — List and send pre-approved WhatsApp templates, essential for initiating conversations with customers
- **Channel Health** — Check your connection status (connected, connecting, disconnected) to ensure your automation is always live
- **Message History** — Retrieve and audit your recent incoming and outgoing message logs to maintain conversation context
- **Interactive Flows** — Handle complex WhatsApp interactions and broadcasts directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your 1msg.io JWT Token
3. Start communicating with your customers on WhatsApp through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Support Teams** — respond to inquiries and send helpful guides on WhatsApp instantly
- **Marketing & Growth** — automate notifications and broadcasts using official templates
- **Operations Managers** — monitor channel status and delivery rates to ensure reliable communications
- **SDRs & Sales** — follow up with leads on their preferred platform without leaving the CRM


## Available Tools
- **send_message**: Requires a recipient phone number and the message body. Do not use for media or templates.

Send a simple WhatsApp text message
- **send_file**: Optionally supports a caption or filename.

Send a media file (image, PDF, video) to a WhatsApp number
- **send_template**: Requires the template name.

Send a pre-approved WhatsApp template message
- **get_status**: g. connected, disconnected). Use this to debug communication failures.

Check the current connection status of the 1msg.io WhatsApp channel
- **list_messages**: Use this to check previous communications or audit chat history.

Retrieve recent incoming and outgoing WhatsApp message history
- **list_templates**: List all available and pre-approved WhatsApp templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **1msg.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message to +123456789 saying: Your order has been shipped!"

**🤖 AI Agent:**
> I've sent the WhatsApp message to +123456789. The message is now being processed by the official 1msg.io gateway.

---

**👤 You:**
> "Send the PDF invoice at https://example.com/inv123.pdf to +123456789 on WhatsApp."

**🤖 AI Agent:**
> I'm sending the PDF document from the provided URL to +123456789. The official 1msg.io gateway will handle the media delivery.

---

**👤 You:**
> "Is my WhatsApp channel connected and working?"

**🤖 AI Agent:**
> Checking your 1msg.io channel status... Your WhatsApp instance is currently 'connected' and ready to send/receive messages.


## ❓ FAQ

**Q: Why do I need to use templates to send a message?**
WhatsApp requires the use of pre-approved templates for any message initiated by the business or sent after 24 hours of the last customer interaction. This prevents spam and ensures high-quality communications.

**Q: Can I send PDF documents or images via the agent?**
Yes! Use the `send_file` tool and provide the recipient's number and the public URL of the document or image. Your agent will handle the formatting and delivery automatically.

**Q: How can I check if my WhatsApp channel is currently online?**
Use the `get_status` tool. It returns the current state of your 1msg.io instance (e.g., connected, connecting, or disconnected). This is crucial for monitoring your automation health.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/1msgio](https://vinkius.com/mcp/1msgio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **1msg.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `1msgio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **1msg.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "1msgio": {
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
