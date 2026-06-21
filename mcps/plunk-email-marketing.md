# Plunk Email Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plunk-email-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate your email marketing via Plunk — send transactional emails, track events, and manage contacts.

## Description
Connect your AI agent to **Plunk**, the versatile email marketing platform designed for developers. This integration allows you to manage your audience, send transactional messages, and track user behavioral events directly through natural conversation.

### What you can do

- **Audience Management** — List, create, and update contacts in your Plunk database, including subscription states
- **Transactional Emails** — Send HTML emails to users for notifications, alerts, or onboarding directly via the agent
- **Event Tracking** — Log custom user actions to trigger automated workflows or segment your audience
- **Campaign & Template Oversight** — List your saved templates and monitor the status of your marketing campaigns
- **Lifecycle Control** — Seamlessly delete contacts or update metadata based on user feedback

### How it works

1. Subscribe to this server
2. Enter your **Plunk Secret Key** (found in your Plunk project settings)
3. Start automating your communication flows via chat

### Who is this for?

- **Growth Marketers** — quickly send test emails or check audience segments
- **Product Managers** — track user events and audit email templates without leaving the conversation
- **Customer Support** — update contact metadata or send direct notifications to users


## Available Tools
- **create_or_update_contact**: Provide metadata as a JSON string if needed.

Create a new contact or update an existing one
- **delete_contact**: Permanently delete a contact from your audience
- **get_contact_details**: Get comprehensive information for a specific contact
- **list_email_campaigns**: Retrieve a list of all email marketing campaigns
- **list_contacts**: Retrieve all contacts in your Plunk audience
- **list_email_templates**: Retrieve a list of all saved email templates
- **send_transactional_email**: Send a transactional email to one or more recipients
- **track_user_event**: Provide data as a JSON string.

Track a custom action performed by a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plunk Email Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in my Plunk audience."

**🤖 AI Agent:**
> Retrieving contacts... I found several users, including 'john@example.com' (Subscribed) and 'jane@example.com' (Unsubscribed).

---

**👤 You:**
> "Send a welcome email to 'test@example.com'."

**🤖 AI Agent:**
> Sending transactional email... Done! The welcome message has been successfully queued for 'test@example.com' with subject 'Welcome to our platform!'.


## ❓ FAQ

**Q: Where do I find my Plunk Secret Key?**
Log in to your [**Plunk Dashboard**](https://app.useplunk.com/), navigate to project settings, and you will find your Secret Key under the API section. It typically starts with `sk_`.

**Q: Can I send bulk newsletters with this agent?**
This integration is optimized for transactional emails and event tracking. For large-scale bulk newsletters, we recommend using the Plunk dashboard or their specialized campaign endpoints for maximum deliverability and compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plunk-email-marketing](https://vinkius.com/mcp/plunk-email-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plunk Email Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plunk-email-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plunk Email Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plunk-email-marketing": {
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
