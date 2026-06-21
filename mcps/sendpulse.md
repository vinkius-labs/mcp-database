# SendPulse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendpulse)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing and automation via SendPulse — handle mailing lists, manage contacts, and track campaigns directly from your AI agent.

## Description
Connect your **SendPulse** account to any AI agent to streamline your email marketing and communication workflows through natural conversation.

### What you can do

- **Mailing Lists** — List, create, update, and delete address books to keep your audience organized.
- **Contact Management** — Add new subscribers, remove contacts, or fetch detailed info for specific email addresses.
- **Campaign Control** — Create and schedule new email campaigns or list existing ones to monitor your outreach.
- **Account Insights** — Instantly check your balance across services (Email, SMTP, Push) and view account owner details.
- **Team Overview** — Retrieve a list of invited users and their roles within your SendPulse organization.

### How it works

1. Subscribe to this server
2. Enter your SendPulse API Key
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — quickly check campaign statuses and manage subscriber lists without switching tabs.
- **Growth Hackers** — automate the process of adding new leads to specific address books via AI.
- **Business Owners** — monitor account balance and team access through simple natural language queries.


## Available Tools (28)
- **add_contacts**: Add contacts to an address book
- **add_smtp_unsubscribe**: Add to SMTP unsubscribe list
- **get_balance**: Get SendPulse balance details
- **create_address_book**: Create a new address book
- **create_campaign**: Create a new email campaign
- **create_crm_contact**: Create a CRM contact
- **create_crm_deal**: Create a CRM deal
- **delete_address_book**: Delete an address book
- **delete_contacts**: Delete contacts from an address book
- **get_campaign_stats**: Get campaign statistics
- **get_chatbot_stats**: Get chatbot stats
- **get_contact_info**: Get contact info from an address book
- **get_smtp_email_details**: Get SMTP email details
- **get_invited_users**: Get invited users list
- **list_address_books**: List all address books (mailing lists)
- **list_campaigns**: Get list of campaigns
- **list_chatbots**: List chatbots
- **list_crm_contacts**: List CRM contacts
- **list_crm_deals**: List CRM deals
- **list_crm_pipelines**: List CRM pipelines
- **list_smtp_emails**: List sent SMTP emails
- **list_smtp_unsubscribes**: Get SMTP unsubscribe list
- **run_chatbot_flow**: Run a chatbot flow for a contact
- **send_chatbot_message**: Send a message to a chatbot contact
- **send_smtp_email**: Send an email via SMTP
- **unsubscribe_contact**: Unsubscribe contacts from an address book
- **update_address_book**: Edit an existing address book
- **get_user_info**: ).

Get SendPulse account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SendPulse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my SendPulse account info and current balance."

**🤖 AI Agent:**
> I've retrieved your account details. Your account is under 'Marketing Team' (Email: admin@company.com). Your current Email service balance is $45.20, and you have 5,000 SMTP credits remaining.

---

**👤 You:**
> "List all my mailing lists and create a new one called 'Leads 2024'."

**🤖 AI Agent:**
> You currently have 3 address books: 'Newsletter', 'Customers', and 'Old Leads'. I have successfully created the new address book 'Leads 2024' with ID 987654.

---

**👤 You:**
> "Get the list of my recent email campaigns."

**🤖 AI Agent:**
> Fetching your campaigns... I found your most recent ones: 'Summer Sale' (Sent), 'Product Update' (Draft), and 'Weekly Digest' (Scheduled). Would you like more details on any of these?


## ❓ FAQ

**Q: How can I check if I have enough credits for a new campaign?**
You can use the `get_balance` tool. It returns the current balance for your main account and specific services like Email, SMTP, and Push notifications.

**Q: Is it possible to add multiple contacts to a mailing list at once?**
Yes! The `add_contacts` tool allows you to pass a JSON array of email objects to bulk-add subscribers to any of your address books.

**Q: Can I see the details of a specific subscriber using their email address?**
Certainly. Use the `get_contact_info` tool by providing the Address Book ID and the specific email address to retrieve their metadata and status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendpulse](https://vinkius.com/mcp/sendpulse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SendPulse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sendpulse` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SendPulse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sendpulse": {
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
