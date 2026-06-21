# UniOne MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unione)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send transactional and bulk emails with high deliverability, detailed analytics, and infrastructure that handles millions of messages.

## Description
Connect your **UniOne** email delivery account to any AI agent and simplify how you manage your transactional messaging, email templates, and delivery tracking through natural conversation.

### What you can do

- **Email Delivery** — Send individual or bulk transactional emails with full HTML support and personalized sender details.
- **Template Automation** — List, create, and send emails using pre-defined templates for consistent branding.
- **Event Monitoring** — Configure webhooks and track delivery events (opened, clicked, delivered) in real-time.
- **Reputation Management** — List and manage suppressed email addresses (unsubscribes/bounces) to protect your sender score.
- **Technical Control** — Fetch detailed metadata for templates and webhooks directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your UniOne API Key and select your Region (eu1 or us1)
3. Start managing your transactional emails from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & DevOps** — quickly test email sending and verify template rendering via simple AI commands.
- **Marketing Operations** — monitor email performance and manage suppression lists directly from the workspace.
- **Product Teams** — automate the creation of notification templates and track user engagement metrics.


## Available Tools (12)
- **delete_template**: Delete a template
- **delete_webhook**: Delete a webhook
- **get_template**: Get template details
- **get_webhook**: Get webhook details
- **list_suppression**: List suppressed emails
- **list_templates**: List email templates
- **list_webhooks**: List webhooks
- **send_email**: Send a transactional email
- **send_template**: Send email using a template
- **set_suppression**: Add email to suppression list
- **set_template**: Create or update a template
- **set_webhook**: Configure a webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UniOne** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all email templates in my UniOne account."

**🤖 AI Agent:**
> I've retrieved your templates. You have 4 active templates: 'Welcome Email', 'Password Reset', 'Order Receipt', and 'Monthly Newsletter'. Which one would you like to inspect?

---

**👤 You:**
> "Send the 'welcome_01' template to 'user@example.com'."

**🤖 AI Agent:**
> Email sent successfully! I've triggered the 'welcome_01' template to user@example.com. The delivery ID is JOB-88231. Shall I track the open status for you?

---

**👤 You:**
> "Check the suppression list for any recent bounces."

**🤖 AI Agent:**
> I've fetched the suppression list. I found 2 recent entries: 'old@example.com' (Hard Bounce) and 'spam@test.com' (Unsubscribed). Shall I add another email to this list?


## ❓ FAQ

**Q: Can I send an email using an existing template ID?**
Yes! Use the `send_template` tool. Provide the Template ID and an array of recipient objects (with their email addresses) to trigger the delivery instantly.

**Q: How do I see which email addresses have been suppressed?**
Run the `list_suppression` query. The agent will retrieve a list of unsubscribed or bounced email addresses managed by your UniOne account.

**Q: Is it possible to update an email template via AI?**
Absolutely. Use the `set_template` action. You can provide the ID, name, subject, and the new HTML body to save changes to your template library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unione](https://vinkius.com/mcp/unione)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UniOne** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unione` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UniOne** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unione": {
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
