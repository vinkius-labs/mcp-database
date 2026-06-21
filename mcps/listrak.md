# Listrak MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/listrak)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email and SMS campaigns, contacts, and messaging via the Listrak REST API.

## Description
Connect your **Listrak** account to any AI agent to automate your cross-channel marketing and transactional messaging. This MCP server enables your agent to manage email and SMS campaigns, interact with contact profiles, and trigger immediate broadcasts directly from natural language interfaces using OAuth 2.0.

### What you can do

- **Email Campaign Management** — List all active and historical email campaigns to monitor your marketing objectives
- **SMS Engagement** — List, create, and manage SMS contacts, and subscribe users to specific phone-based lists
- **Transactional Messaging** — Trigger pre-defined transactional emails instantly for order confirmations, alerts, or notifications
- **Instant Broadcasts** — Send immediate SMS broadcast messages to your audience using your configured sender codes
- **Contact Insights** — Retrieve detailed profile information for email contacts across your organizational lists
- **Database Maintenance** — Create new SMS profiles and manage cross-channel subscriptions effortlessly

### How it works

1. Subscribe to this server
2. Enter your Listrak Client ID and Client Secret
3. Start managing your cross-channel marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **CRM Managers** — Monitor campaign statuses and manage subscriber lists via simple natural language commands
- **Marketing Operations** — Quickly trigger transactional alerts and verify contact data without opening the portal
- **Growth Engineers** — Integrate email and SMS automation logic directly into your custom internal tools


## Available Tools
- **send_sms_broadcast**: Send an immediate SMS broadcast
- **create_sms_contact**: Add a new SMS contact
- **list_email_campaigns**: List all email campaigns
- **get_email_contact_details**: Get details for a specific email contact
- **list_sms_contacts**: List SMS contacts
- **send_transactional_email**: Requires messageId and recipient data.

Send a transactional email
- **subscribe_to_sms_list**: Subscribe a contact to an SMS list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Listrak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current email campaigns in Listrak."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 active campaigns, including 'Winter Sale (ID: 123)' and 'Newsletter Monthly (ID: 456)'. Would you like to see details for any of them?

---

**👤 You:**
> "Send a transactional email (Message ID: '987') to 'user@example.com'."

**🤖 AI Agent:**
> I've triggered the transactional email for user@example.com using message template 987. Listrak has queued the delivery.

---

**👤 You:**
> "Subscribe the phone number '+15550199' to SMS list '555'."

**🤖 AI Agent:**
> Successfully subscribed +15550199 to your SMS list 555. The contact will now receive messages according to your list's automation rules.


## ❓ FAQ

**Q: How do I find my ListID and MessageID?**
In the Listrak platform, navigate to Help & Support > API ID Information. All IDs for your lists, profile fields, and messages are displayed there.

**Q: Is IP whitelisting required for the Listrak API?**
Yes, Listrak requires you to whitelist the calling IP addresses in the Integration Management section of your account for the API to function correctly.

**Q: Can I send SMS to an international phone number?**
Yes, as long as your Listrak account and sender code are configured for international messaging. Ensure the phone number is provided in E.164 format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listrak](https://vinkius.com/mcp/listrak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Listrak** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `listrak` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Listrak** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "listrak": {
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
