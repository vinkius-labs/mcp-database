# Loops MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loops)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Email marketing and transactional email platform with powerful automation, audience segmentation, and analytics.

## Description
Loops is a modern email marketing and transactional email platform designed for startups and growing businesses. It provides powerful automation for email journeys, audience segmentation, contact management, and detailed analytics. This MCP server enables AI agents to manage contacts, mailing lists, trigger events for automated journeys, send transactional emails, and check suppression statuses — all through natural language commands.

**Key capabilities:**
- Search, create, update, and delete contacts
- Manage mailing lists
- Trigger email journeys with events
- Send transactional emails programmatically
- Check email suppression status
- View sent transactional email history


## Available Tools (10)
- **create_contact**: Requires an email address. Optionally accepts firstName, lastName, and userGroup.

Create a new contact in Loops
- **delete_contact**: This action cannot be undone.

Delete a contact from Loops by ID
- **find_contact**: Returns the contact details if found.

Find a contact in Loops by email address
- **get_contact_suppression**: Suppressed emails will not receive emails. Returns the suppression status for the given email.

Check if an email address is suppressed in Loops
- **list_mailing_lists**: Use this to discover available lists for subscribing contacts.

List all mailing lists in Loops
- **list_transactional_emails**: Optionally accepts a limit parameter to control the number of results returned.

List recently sent transactional emails from Loops
- **send_event**: Requires an eventName. Optionally accepts email and/or userId to identify the recipient.

Send an event to trigger email journeys in Loops
- **send_transactional_email**: Requires the transactionalId. Optionally accepts email and dataVariables (as JSON string) for template variables.

Send a transactional email via Loops
- **test_api_key**: Returns success/failure status.

Test if the Loops API key is valid and working
- **update_contact**: Requires the contact ID. Accepts any fields to update such as firstName, lastName, email, userGroup, etc.

Update an existing contact in Loops by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loops** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the contact with email user@example.com in Loops"

**🤖 AI Agent:**
> I searched for the contact with email user@example.com in Loops and found it. Here are the contact details including subscription status and attributes.

---

**👤 You:**
> "Create a new contact in Loops with email newuser@example.com, first name John, and last name Doe"

**🤖 AI Agent:**
> I created a new contact in Loops with the email newuser@example.com and name John Doe. The contact has been successfully added to your Loops account.

---

**👤 You:**
> "List all mailing lists in my Loops account"

**🤖 AI Agent:**
> Here are all the mailing lists configured in your Loops account. You can use these lists to manage subscribers and send campaigns.

---

**👤 You:**
> "Send a transactional email with template txn_123 to customer@example.com"

**🤖 AI Agent:**
> I sent the transactional email using template txn_123 to customer@example.com. The email has been queued for delivery.

---

**👤 You:**
> "Send a 'user-signed-up' event for email newuser@example.com to trigger the welcome journey"

**🤖 AI Agent:**
> I sent the 'user-signed-up' event for newuser@example.com. This will trigger the welcome email journey in Loops.


## ❓ FAQ

**Q: How do I get a Loops API key?**
Log in to your Loops account, go to **Settings** → **API**, and generate a new API key. Ensure it has the necessary permissions. Then provide it when prompted by the MCP server setup.

**Q: What operations are supported by this MCP server?**
The server supports: testing API key validity, finding/creating/updating/deleting contacts, listing mailing lists, sending events to trigger email journeys, sending transactional emails, listing sent transactional emails, and checking contact suppression status.

**Q: What is the difference between mailing lists and transactional emails in Loops?**
Mailing lists are used for marketing campaigns and automated email journeys. Transactional emails are one-off, triggered messages like receipts, password resets, or order confirmations. Both are supported by this MCP server.

**Q: How can I check if an email is suppressed in Loops?**
Use the 'get_contact_suppression' tool provided by this MCP server. Simply ask the AI to check the suppression status for any email address, and it will tell you if that email is currently suppressed from receiving emails.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loops](https://vinkius.com/mcp/loops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loops** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `loops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loops** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loops": {
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
