# QuickReply.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickreplyai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate WhatsApp marketing and customer engagement via QuickReply.ai — trigger journeys, send templates, and manage session messages directly from your AI agent.

## Description
Connect **QuickReply.ai** to your AI agent and orchestrate your WhatsApp marketing and customer communication through natural conversation.

### What you can do

- **Automated Journeys** — Trigger personalized WhatsApp journeys using the `trigger_journey_event` tool with specific receiver IDs.
- **Template Messaging** — Send pre-approved WhatsApp templates with dynamic variables using `send_template` for official notifications.
- **Session Conversations** — Send free-form text and images within the 24-hour service window using `send_session_message`.
- **Drip Campaigns** — Schedule and trigger automated drip sequences for user nurturing with `trigger_drip_campaign`.
- **Performance Analytics** — Retrieve detailed message-level statistics and insights using `fetch_campaign_stats`.

### How it works

1. Subscribe to this server
2. Enter your QuickReply.ai Client ID and Secret Key
3. Start managing your WhatsApp outreach from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Launch campaigns and track performance without switching between multiple dashboards.
- **Customer Support Teams** — Respond to users with session messages and send automated updates via templates.
- **Sales & Growth Leads** — Automate lead nurturing journeys and follow-up sequences directly through AI orchestration.


## Available Tools (5)
- **fetch_campaign_stats**: Note: This API will sunset in June 2026.

Fetch campaign messages stats
- **send_session_message**: Send a free-form session message
- **send_template**: Send a pre-approved WhatsApp template
- **trigger_drip_campaign**: Note: This API will sunset in June 2026.

Trigger a specific drip campaign for a user
- **trigger_journey_event**: This is the recommended way to trigger messages.

Trigger a journey via Webhook Data Source


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuickReply.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger the WhatsApp journey 'welcome_flow_01' for phone +1234567890."

**🤖 AI Agent:**
> I've triggered the journey 'welcome_flow_01' for +1234567890. The event has been successfully sent to the QuickReply.ai engine.

---

**👤 You:**
> "Send the 'order_confirmation' template to +1234567890 with parameters 'Order #123' and 'Confirmed'."

**🤖 AI Agent:**
> The order confirmation template has been sent to +1234567890 with the provided variables.

---

**👤 You:**
> "Fetch campaign statistics for the last 24 hours."

**🤖 AI Agent:**
> I've retrieved the stats for your campaigns. In the last 24 hours, you had 1,250 messages sent with a 98% delivery rate and 45% read rate.


## ❓ FAQ

**Q: Can I trigger a WhatsApp journey using a webhook receiver ID?**
Yes! Use the `trigger_journey_event` tool with the specific receiver ID generated from your Webhook Data Source. You can also pass custom fields to personalize the journey.

**Q: How do I send a pre-approved WhatsApp template with variables?**
Use the `send_template` tool. Provide the `template_id`, the recipient's phone number, and an array of `params` to replace the variables in your template body.

**Q: Can I send free-form text messages to customers?**
Yes, as long as it is within the 24-hour service window. Use the `send_session_message` tool to send text and optional images to your users.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickreplyai-alternative](https://vinkius.com/mcp/quickreplyai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuickReply.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quickreplyai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuickReply.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quickreplyai-alternative": {
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
