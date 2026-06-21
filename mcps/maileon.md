# Maileon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maileon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing contacts, mailings, and reporting via the Maileon REST API.

## Description
Connect your **Maileon** account to any AI agent to automate your professional email marketing and audience management. This MCP server enables your agent to manage subscribers, control mailing lifecycles, and retrieve detailed performance statistics directly from natural language interfaces.

### What you can do

- **Contact Management** — List all subscribers, retrieve complete profiles by email, and manage opt-ins and opt-outs
- **Mailing Control** — Monitor your email campaigns (mailings), retrieve metadata, and trigger official dispatches when ready
- **Real-time Reporting** — Retrieve KPIs and statistics for individual mailings, including opens, clicks, and bounces
- **Audience Hygiene** — Monitor unsubscription events and permanently remove contacts to maintain list quality
- **Data Ingestion** — Create and update subscriber records programmatically to sync with your external CRMs

### How it works

1. Subscribe to this server
2. Enter your Maileon REST API Key
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **CRM Managers** — Monitor campaign statuses and manage subscriber lists via simple natural language commands
- **Marketing Operations** — Quickly check mailing performance and manage contact updates without opening the portal
- **Developers** — Integrate Maileon's advanced mailing logic and reporting into your custom internal tools


## Available Tools
- **list_account_contacts**: Use optional params for filtering.

List all contacts in the Maileon account
- **create_new_contact**: Can trigger a Double Opt-In process if configured.

Add or update a contact in the database
- **delete_account_contact**: Remove a contact from the account
- **dispatch_email_mailing**: The mailing must be in a ready state.

Trigger the dispatch of a mailing
- **get_contact_by_email**: Get details for a specific contact
- **get_mailing_details**: Get details for a specific mailing
- **get_mailing_statistics**: Get performance statistics for a mailing
- **list_email_mailings**: Use optional params to filter by state (e.g., "state=draft").

List all mailings (campaigns)
- **list_unsubscription_events**: List recent unsubscription events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maileon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active mailings in my Maileon account."

**🤖 AI Agent:**
> I've retrieved your mailings. You have 5 campaigns, including 'Summer Newsletter (ID: 12345)', 'Product Launch', and 'Welcome Sequence'. Which one would you like to see statistics for?

---

**👤 You:**
> "Get the latest statistics for mailing ID '12345'."

**🤖 AI Agent:**
> I've fetched the statistics for mailing 12345. Currently, it has a 25.4% open rate and a 3.2% click-through rate across 10,000 recipients.

---

**👤 You:**
> "Add 'new-user@example.com' to my Maileon contacts."

**🤖 AI Agent:**
> Successfully created the contact record for new-user@example.com. The new subscriber is now registered in your database.


## ❓ FAQ

**Q: How do I find my Maileon API Key?**
Log in to your Maileon account and navigate to Settings > API to generate and copy your unique REST API Key.

**Q: What is the difference between a Mailing and a Campaign?**
In Maileon terminology, a 'Mailing' refers to a specific email send-out, which is the standard entity managed via the campaigns tools in this server.

**Q: Can I filter contacts by specific attributes?**
Yes, you can provide filtering strings in the `params` field of the `list_account_contacts` tool following the Maileon query syntax.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maileon](https://vinkius.com/mcp/maileon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maileon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `maileon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maileon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maileon": {
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
