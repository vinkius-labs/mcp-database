# MailerLite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailerlite-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate email marketing via MailerLite — manage subscribers, organize groups, and track campaign activity directly from any AI agent.

## Description
Connect your **MailerLite** account to any AI agent to streamline your email marketing and subscriber management through natural conversation.

### What you can do

- **Subscriber Management** — List, create, update, and fetch detailed profiles for your audience members
- **Audience Organization** — Manage subscriber groups and segments to ensure targeted and relevant communication
- **Activity Tracking** — Monitor subscriber engagement and activity logs to understand user behavior
- **Campaign Insights** — Access campaign data and automation workflows to stay on top of your marketing performance
- **GDPR Compliance** — Securely handle 'forget' requests to maintain data privacy standards

### How it works

1. Subscribe to this server
2. Enter your MailerLite API Key
3. Start managing your email lists and campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — quickly check subscriber counts, group status, and campaign performance without logging into the dashboard
- **Growth Hackers** — automate the process of adding new leads to specific groups directly from research or chat workflows
- **Support Teams** — instantly verify subscriber status and activity history to provide better customer context


## Available Tools (51)
- **create_automation**: Create a draft automation
- **create_campaign**: Create a campaign
- **create_field**: Create a custom field
- **create_group**: Create a new group
- **create_shop**: Create an e-commerce shop
- **create_subscriber**: Create or upsert a subscriber
- **create_webhook**: Create a webhook
- **delete_automation**: Delete an automation
- **delete_campaign**: Delete a campaign
- **delete_field**: Delete a custom field
- **delete_form**: Delete a form
- **delete_group**: Delete a group
- **delete_segment**: Delete a segment
- **delete_shop**: Delete an e-commerce shop
- **delete_subscriber**: Delete a subscriber
- **delete_webhook**: Delete a webhook
- **forget_subscriber**: Forget a subscriber (GDPR)
- **get_automation_activity**: Get automation activity
- **get_automation**: Get automation details
- **get_campaign_activity**: Get campaign activity report
- **get_campaign**: Get campaign details
- **get_form**: Get form details
- **get_subscriber_activity**: Get subscriber activity log
- **get_subscriber**: Get a specific subscriber
- **import_subscribers_to_group**: Import subscribers to a group
- **list_automations**: List all automations
- **list_campaign_languages**: List supported campaign languages
- **list_campaigns**: List all campaigns
- **list_fields**: List all custom fields
- **list_form_subscribers**: List form subscribers
- **list_forms**: List forms by type
- **list_group_subscribers**: List subscribers in a group
- **list_groups**: List all groups
- **list_segment_subscribers**: List subscribers in a segment
- **list_segments**: List all segments
- **list_shops**: List all e-commerce shops
- **list_subscribers**: Can be filtered by status.

List all subscribers
- **list_timezones**: List supported timezones
- **list_webhooks**: List all webhooks
- **schedule_campaign**: Schedule a campaign
- **unassign_subscriber_from_group**: Unassign subscriber from a group
- **update_campaign**: Update a campaign
- **update_field**: Update a custom field
- **update_form**: Update a form
- **update_group**: Update a group
- **update_segment**: Update a segment
- **update_shop**: Update an e-commerce shop
- **assign_subscriber_to_group**: Assign subscriber to a group
- **cancel_campaign**: Cancel a campaign
- **update_subscriber**: Update a subscriber
- **update_webhook**: Update a webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerLite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active subscribers."

**🤖 AI Agent:**
> I've retrieved your active subscribers. You have 1,240 active members. The most recent additions include 'john.doe@example.com' and 'jane.smith@work.com'.

---

**👤 You:**
> "Get details for subscriber test@example.com."

**🤖 AI Agent:**
> Found them! Subscriber 'test@example.com' (ID: 987654) is currently 'active'. They are part of the 'Early Adopters' group and were last updated on October 12th.

---

**👤 You:**
> "Show me all my subscriber groups."

**🤖 AI Agent:**
> You have 4 groups configured: 'Newsletter' (ID: 111), 'VIP Customers' (ID: 222), 'Webinar Leads' (ID: 333), and 'Uncategorized' (ID: 444).


## ❓ FAQ

**Q: Can I find a specific subscriber using their email address?**
Yes! Use the `get_subscriber` tool and provide the email address. The agent will return the subscriber's ID, status, and custom field data.

**Q: How do I see what a subscriber has been doing recently?**
You can use the `get_subscriber_activity` tool with the subscriber's ID. This will show you opens, clicks, and other interactions recorded in MailerLite.

**Q: Is there a way to comply with GDPR 'Right to be Forgotten' requests?**
Absolutely. Use the `forget_subscriber` tool with the subscriber's ID to completely and permanently delete their data from your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailerlite-alternative-1](https://vinkius.com/mcp/mailerlite-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailerLite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailerlite-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailerLite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailerlite-alternative-1": {
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
