# Brevo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brevo-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate transactional messaging via Brevo — send emails, SMS, and WhatsApp messages, manage templates, and track delivery statistics directly from any AI agent.

## Description
Connect your **Brevo** account to any AI agent to orchestrate your transactional communication and marketing workflows through natural conversation.

### What you can do

- **Transactional Email** — Send emails using JSON payloads, list sent messages, and retrieve detailed content for specific message IDs.
- **Template Management** — List, create, update, and fetch details for email templates to maintain consistent branding.
- **Multi-Channel Messaging** — Send transactional SMS and WhatsApp messages directly through the API.
- **Advanced Analytics** — Access aggregated statistics reports and unaggregated event logs for both Email and SMS activity.
- **Scheduled Control** — Manage your queue by deleting scheduled transactional emails before they are sent.

### How it works

1. Subscribe to this server
2. Enter your Brevo API Key (v3)
3. Start sending messages and analyzing reports from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate transactional notifications and debug email delivery logs without leaving the terminal or IDE.
- **Marketing Operations** — manage email templates and monitor campaign performance through simple queries.
- **Customer Support** — verify if specific transactional emails were delivered to users by checking message IDs and event logs.


## Available Tools
- **create_contact_attribute**: Create a new contact attribute
- **create_contact_folder**: Create a new contact folder
- **create_contact_list**: Create a new contact list
- **create_contact**: Create a new contact
- **create_email_campaign**: Create an email campaign
- **create_email_template**: Create a new email template
- **create_event**: Create a single event (e.g., for tracking website activity)
- **create_events_batch**: Create events in batch
- **create_sender**: Create a new sender
- **create_sms_campaign**: Create an SMS campaign
- **create_webhook**: Create a new webhook
- **delete_contact**: Delete a contact
- **delete_scheduled_email**: Delete a scheduled email
- **get_account_activity**: Get user activity logs
- **get_account**: Get general account information and credits
- **get_contact**: Get details of a specific contact
- **get_email_statistics_events**: Get unaggregated transactional email activity (logs)
- **get_email_statistics_reports**: Get aggregated transactional email activity per day
- **get_email_template**: Get details of a specific email template
- **get_sms_campaign**: Get details of an SMS campaign
- **get_sms_statistics_events**: Get unaggregated SMS activity logs
- **get_sms_statistics_reports**: Get aggregated SMS activity
- **get_transactional_email**: Get personalized content of a sent email
- **get_webhook**: Get details of a webhook
- **get_whatsapp_statistics_events**: Get unaggregated WhatsApp activity logs
- **list_contact_attributes**: List all contact attributes
- **list_contact_folders**: List all contact folders
- **list_contact_lists**: List all contact lists
- **list_contacts**: List all contacts
- **list_domains**: List all sender domains
- **list_email_campaigns**: List all email campaigns
- **list_email_templates**: List all email templates
- **list_events**: Retrieve tracked events
- **list_senders**: List all verified email senders
- **list_sms_campaigns**: List all SMS campaigns
- **list_transactional_emails**: Get a list of transactional emails
- **list_webhooks**: List all configured webhooks
- **register_domain**: Register a new domain
- **send_email_campaign_now**: Send an email campaign immediately
- **send_transactional_email**: Send a transactional email
- **send_transactional_sms**: Send a transactional SMS
- **send_whatsapp_message**: Send a WhatsApp message
- **update_contact**: Update a contact
- **update_email_campaign**: Update an email campaign
- **update_email_template**: Update an existing email template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brevo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email to contact@example.com with the subject 'Order Confirmed' and HTML content 'Your order #123 is on its way!'"

**🤖 AI Agent:**
> I've sent the transactional email. The message has been queued successfully and assigned a message ID for tracking.

---

**👤 You:**
> "List all my current email templates in Brevo."

**🤖 AI Agent:**
> I've retrieved your templates. You have 4 active templates, including 'Welcome Series', 'Password Reset', and 'Monthly Newsletter'. Would you like to see the details for any of them?

---

**👤 You:**
> "Show me the statistics for my SMS activity from the last 30 days."

**🤖 AI Agent:**
> Fetching SMS reports... In the last 30 days, you sent 150 messages with a 98% delivery rate and 0% hard bounces. Would you like to see the unaggregated event logs for more detail?


## ❓ FAQ

**Q: Can I send a custom transactional email using a JSON payload?**
Yes! Use the `send_transactional_email` tool. You can provide a full JSON payload including sender details, recipients, subject line, and HTML content to trigger an immediate delivery.

**Q: How do I check the performance of my email activity for a specific period?**
You can use the `get_email_statistics_reports` tool. It provides aggregated transactional email activity per day, allowing you to filter by date or other optional parameters.

**Q: Is it possible to manage my email templates directly through the AI?**
Absolutely. You have access to a full suite of tools: `list_email_templates` to see what's available, `create_email_template` to build new ones, and `update_email_template` to modify existing designs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brevo-alternative-1](https://vinkius.com/mcp/brevo-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brevo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `brevo-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brevo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brevo-alternative-1": {
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
