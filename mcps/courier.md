# Courier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/courier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to send multi-channel notifications and monitor delivery status through the Courier API.

## Description
Integrate **Courier**, the smart notification infrastructure, directly into your AI workflow. Design, orchestrate, and send messages across email, SMS, push, and chat apps using natural language.

### What you can do

- **Send Notifications** — Trigger complex notification workflows to any recipient via the Send API.
- **Message Monitoring** — List sent messages and track their real-time delivery status (sent, delivered, opened).
- **Template Management** — Browse available notification templates and custom brands.
- **Audience & User Insights** — Manage subscription lists and retrieve user profiles.

### How it works

1. Connect the Courier integration to your AI assistant.
2. Authorize using your Courier Auth Token (found in Settings > API Keys).
3. Manage your global notification strategy through chat.

### Who is this for?

- **Product Managers** — Quickly verify if critical system notifications are being delivered.
- **Developers** — Audit message history and troubleshoot delivery issues via chat.
- **Customer Support** — Check user profiles and their recent notification history to provide better help.


## Available Tools
- **get_message_history**: Resolves event types (SENT, DELIVERED, etc.) and detailed provider logs.

Get the delivery history logs for a message
- **get_message_details**: Touches delivery logs, provider responses, and rendering metadata boundary.

Get details for a specific message by ID
- **get_user_profile**: Resolves contact details (email, phone) and channel-specific delivery preferences.

Get the profile data for a specific user
- **list_audiences**: Resolves audience IDs, names, and filter criteria used for segmentation.

List saved audiences for targeted notifications
- **list_brands**: Resolves brand names, colors, and logo settings used for white-labeling notifications.

List custom brands configured in Courier
- **list_subscription_lists**: Resolves list IDs, names, and subscriber counts.

List subscription lists for managing recipients
- **list_messages**: Resolves message IDs, recipient identifiers, status (SENT, DELIVERED, OPENED, CLICKED), and timestamps.

List sent messages and their current status
- **list_templates**: Resolves template names, IDs, and supported channels.

List available notification templates
- **list_users**: Resolves user IDs, roles, and account association details.

List users registered in the Courier workspace
- **send_notification**: Touches recipient profile, template engine, and multi-channel provider boundaries.

Send a notification to a recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Courier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the delivery status of the last message sent to 'user@example.com'."

**🤖 AI Agent:**
> The last message sent to 'user@example.com' (Request ID: 8s9df7) has been successfully 'DELIVERED' via SendGrid. It was opened 5 minutes ago. Would you like to see the full event history?

---

**👤 You:**
> "Send a 'Welcome' notification to the new user with ID 'user_123'."

**🤖 AI Agent:**
> I've enqueued the 'Welcome' notification for user 'user_123'. Courier will route it through the best available channel. Should I monitor the delivery status for you?

---

**👤 You:**
> "List all notification templates available in my account."

**🤖 AI Agent:**
> I've retrieved 15 templates, including 'Password Reset', 'New Login Alert', and 'Monthly Digest'. Would you like to see the details for a specific template?


## ❓ FAQ

**Q: How do I get a Courier Auth Token?**
Log in to your Courier dashboard, navigate to **Settings > API Keys**, and you will find your Auth Token there. Use the 'Published' key for production environments.

**Q: What channels are supported?**
Courier supports dozens of providers for Email (SendGrid, Mailgun), SMS (Twilio, MessageBird), Push (Firebase, OneSignal), and Chat (Slack, Discord).

**Q: Can I track if a message was opened?**
Yes, the agent can use the get_message_details tool to check the status of a specific message, which includes tracking events like 'OPENED' or 'CLICKED' if supported by the provider.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/courier](https://vinkius.com/mcp/courier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Courier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `courier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Courier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "courier": {
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
