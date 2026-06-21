# WhatsApp Business MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whatsapp-business-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate your customer communication — send templates and manage profiles via AI.

## Description
Empower your AI agent to orchestrate your entire mobile communication strategy with the **WhatsApp Business Platform**, the world's most popular messaging tool. By connecting WhatsApp to your agent, you transform enterprise messaging into a natural conversation. Your agent can instantly send pre-approved templates, audit your business profile, and manage message templates without you ever touching a complex Meta dashboard. Whether you are providing customer support or running a global notification system, your agent acts as a real-time communication manager, ensuring your brand is always reachable and responsive.

### What you can do

- **Template Messaging** — Send pre-approved, highly structured templates to your customers with dynamic variables.
- **Free-Text Communication** — Send direct text messages to users within active customer service windows.
- **Business Auditing** — Retrieve your public business profile, phone number details, and account metadata instantly.
- **Template Governance** — List all message templates and autonomously delete those that are no longer needed.
- **Media Insights** — Retrieve metadata for images and documents shared through your WhatsApp Business Account.

### How it works

1. Subscribe to this server
2. Enter your Meta Access Token, WABA ID, and Phone Number ID
3. Start communicating with your customers through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — monitor communication profiles and send quick updates straight from your workflow.
- **Marketing Leads** — verify if message templates have been correctly approved and are ready for distribution.
- **IT Support Teams** — perform rapid account health checks and manage phone numbers without manual Meta logins.
- **Operations Managers** — automate messaging workflows to orchestrate customer engagement smoothly.


## Available Tools
- **delete_message_template**: Delete a WhatsApp template
- **get_business_profile**: Get WhatsApp business profile
- **get_media**: Get media information
- **get_waba_details**: Get WABA account details
- **list_message_templates**: List WhatsApp message templates
- **list_phone_numbers**: List WhatsApp phone numbers
- **send_template_message**: Send a WhatsApp template message
- **send_text_message**: Note: This usually requires an active customer service window.

Send a WhatsApp text message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WhatsApp Business** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my WhatsApp phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' (Main Business) and '+1 987 654 321' (Support). Which one would you like to use?

---

**👤 You:**
> "Send the 'welcome_offer' template to +5511999999999."

**🤖 AI Agent:**
> Template message sent! I've successfully delivered the 'welcome_offer' to +5511999999999. The message ID is wamid.HBgLNTU...

---

**👤 You:**
> "Show me my current WhatsApp message templates."

**🤖 AI Agent:**
> I've found 4 templates in your account: 'order_update', 'shipping_notice', 'welcome_offer', and 'feedback_request'. All are currently approved and ready for use.


## ❓ FAQ

**Q: How do I find my Phone Number ID and WABA ID?**
Log in to your [**Meta App Dashboard**](https://developers.facebook.com/apps/), select your app, and navigate to **WhatsApp** > **Getting Started**. You will find both IDs and your Access Token there.

**Q: Can I send messages to any WhatsApp user?**
You can send pre-approved templates at any time. However, to send free-text messages, the user must have interacted with your business in the last 24 hours.

**Q: What happens if a message template is not approved?**
Unapproved templates cannot be sent via the API. You can check the status of your templates using the `list_message_templates` tool to verify their readiness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whatsapp-business-alternative](https://vinkius.com/mcp/whatsapp-business-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WhatsApp Business** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `whatsapp-business-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WhatsApp Business** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whatsapp-business-alternative": {
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
