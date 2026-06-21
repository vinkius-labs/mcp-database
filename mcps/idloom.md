# idloom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/idloom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage events, attendees, and invoices via idloom.events API.

## Description
Empower your AI agents to manage your events ecosystem with idloom.events. This MCP server allows you to list and retrieve events, manage attendees, track invoices, and view transactions directly through the idloom API. Ideal for automating event logistics and registration workflows.


## Available Tools
- **get_attendee**: Retrieves details for a specific attendee
- **get_event**: Retrieves details for a specific event
- **list_attendees**: Lists all attendees
- **list_categories**: Lists all categories
- **list_emails**: Lists all emails
- **list_events**: Lists all events managed in idloom
- **list_invoices**: Lists all invoices
- **list_registration_forms**: Lists all registration forms
- **list_transactions**: Lists all transactions
- **list_webhooks**: Lists all webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **idloom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in my idloom account."

**🤖 AI Agent:**
> I'll fetch the list of events for you.

---

**👤 You:**
> "Show me the attendee list for event ID '123'."

**🤖 AI Agent:**
> I'll retrieve the attendee list for that specific event.

---

**👤 You:**
> "Check for any unpaid invoices."

**🤖 AI Agent:**
> I'll look up your invoices and highlight any that are pending payment.


## ❓ FAQ

**Q: How do I get idloom API credentials?**
Log in to your idloom.events backend, navigate to Integrations, create a Custom Integration, and enable API access to generate your unique Bearer Token.

**Q: Which version of the API is used?**
This MCP uses idloom API v4, the latest stable version for event and attendee management.

**Q: Can I see attendee check-ins?**
Yes, the list_attendees tool provides access to attendee details including their registration and status information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/idloom](https://vinkius.com/mcp/idloom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **idloom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `idloom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **idloom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "idloom": {
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
