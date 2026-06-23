# Eventzilla MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventzilla-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Event management and ticketing platform — manage registrations, attendees, and check-ins via AI.

## Description
Empower your AI agent to orchestrate your entire event ecosystem with **Eventzilla**, the leading platform for event registration and marketing. By connecting Eventzilla to your agent, you transform complex event logistics into a natural conversation. Your agent can instantly list upcoming events, audit attendee lists, and perform real-time check-ins without you ever touching a dashboard. Whether you are managing a small workshop or a large-scale conference, your agent acts as a real-time event operations manager, ensuring your registrations are always tracked and accessible.

### What you can do

- **Event Directory** — List all events in your account, filter by status, and inspect detailed event metadata.
- **Attendee Management** — Fetch complete attendee profiles, registration answers, and monitor real-time check-in status.
- **Ticketing & Sales** — Query different ticket types, monitor transaction history, and audit financial orders for any event.
- **On-site Operations** — Perform digital check-ins using barcodes and manage attendee entry flows directly from chat.
- **Promo & Customization** — List active discount codes and retrieve custom registration questions to analyze your audience.

### How it works

1. Subscribe to this server
2. Enter your Eventzilla API Key
3. Start managing your event data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — instantly retrieve registration counts, audit attendee profiles, and manage check-ins without manual dashboard logins.
- **Marketing Teams** — monitor the performance of discount codes and analyze attendee demographics through registration questions.
- **On-site Staff** — perform rapid check-ins and verify ticket validity directly through a mobile-friendly AI interface.
- **Financial Controllers** — track event revenue and transaction history through simple natural language queries.


## Available Tools (11)
- **checkin_attendee**: Check-in an attendee
- **get_attendee**: Get attendee details
- **get_event**: Get details for a specific event
- **get_transaction**: Get transaction details
- **list_attendees**: List attendees for an event
- **list_categories**: g., Business, Music).

List event categories
- **list_discount_codes**: List discount codes for an event
- **list_events**: List all events
- **list_questions**: List registration questions
- **list_tickets**: List tickets for an event
- **list_transactions**: List transactions for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventzilla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all live events in my account."

**🤖 AI Agent:**
> I've retrieved your live events. You currently have 3 active events: 'Global Tech Summit 2024', 'AI Workshop Series', and 'Networking Night'. Which one would you like to drill into?

---

**👤 You:**
> "Fetch the attendee list for event ID 987654."

**🤖 AI Agent:**
> I've retrieved the attendee list for that event. There are 120 registered participants. Notable names include 'Mark Thompson' and 'Sarah Jenkins'. Would you like the check-in status for any of them?

---

**👤 You:**
> "Show the transaction history for event 'Global Tech Summit'."

**🤖 AI Agent:**
> Fetching transaction records... For the 'Global Tech Summit', I found 85 successful orders totaling $12,500 in revenue. I can list the specific reference numbers and amounts if needed.


## ❓ FAQ

**Q: How do I check if an attendee has checked in?**
Use the `get_attendee` tool with the attendee ID. The response will include the check-in status and timestamp if they are already on-site.

**Q: Can I perform a check-in directly through the AI agent?**
Yes! Use the `checkin_attendee` tool by providing the attendee's barcode. You can also revert a check-in by setting the `eventcheckin` parameter to 'false'.

**Q: How do I see all ticket sales for a specific event?**
Use the `list_transactions` tool with the target Event ID. It will return a full history of all financial orders and transaction details for that event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventzilla-alternative](https://vinkius.com/mcp/eventzilla-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eventzilla** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eventzilla-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eventzilla** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventzilla-alternative": {
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
