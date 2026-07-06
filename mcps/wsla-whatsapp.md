# WSLA (WhatsApp) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wsla-whatsapp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send WhatsApp messages, templates, and reactions via AI using the Meta Cloud API.

## Description
Connect your **WhatsApp Business Platform** (via Meta Cloud API) to any AI agent to automate your customer communications. WSLA provides a direct bridge to Meta's infrastructure for reliable, scalable messaging.

### What you can do

- **Conversational AI** — Send instant text messages to any WhatsApp number during active customer support windows.
- **Business Notifications** — Use pre-approved message templates for proactive alerts, appointment reminders, and shipping updates.
- **Interactive Reactions** — Allow your AI agent to react to incoming customer messages with emojis for more natural engagement.
- **Template Management** — List and search all approved templates associated with your WhatsApp Business Account.
- **Media Intelligence** — Retrieve details for incoming media to enable multi-modal interactions through your AI agent.

### How it works

1. Subscribe to this server
2. Enter your Meta System User Access Token and WhatsApp Phone Number ID
3. Start automating your WhatsApp engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — automate common customer queries and proactive status updates.
- **Marketing Operations** — send personalized template-based notifications to your opted-in audience.
- **Developers** — integrate real-time WhatsApp messaging into custom AI-driven business workflows.


## Available Tools (5)
- **get_whatsapp_media_details**: Get media details
- **list_whatsapp_templates**: List message templates
- **send_whatsapp_template**: Send a WhatsApp template message
- **send_whatsapp_text**: Send a text message via WhatsApp
- **send_whatsapp_reaction**: React to a WhatsApp message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WSLA (WhatsApp)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp message 'Welcome to our service!' to +1234567890."

**🤖 AI Agent:**
> Message sent successfully! I've triggered the welcome notification to the recipient via WhatsApp Cloud API.

---

**👤 You:**
> "List all approved templates for my business account."

**🤖 AI Agent:**
> I've retrieved your templates. You have 10 approved message templates, including 'shipping_update', 'appointment_reminder', and 'welcome_pack'.


## ❓ FAQ

**Q: Where do I find my Phone Number ID and Access Token?**
Log in to the [**Meta Developer Portal**](https://developers.facebook.com/), select your App, and navigate to the WhatsApp > Getting Started section for the ID, and the App Settings for the System User Access Token.

**Q: What is the 24-hour window policy?**
WhatsApp restricts business-initiated free-text messages. You can only send free-form text if the user has messaged you in the last 24 hours. Outside this window, you must use a pre-approved Template.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wsla-whatsapp](https://vinkius.com/mcp/wsla-whatsapp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WSLA (WhatsApp)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wsla-whatsapp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WSLA (WhatsApp)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wsla-whatsapp": {
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
