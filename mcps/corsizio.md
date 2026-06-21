# Corsizio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corsizio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage event registrations, attendees, and payments through the Corsizio API.

## Description
Integrate **Corsizio**, the streamlined event registration platform, directly into your AI workflow. Manage your classes, workshops, and seminars, track attendee lists, and monitor revenue using natural language.

### What you can do

- **Event Management** — List and retrieve details for all your upcoming and past events.
- **Attendee Tracking** — Quickly access registration lists and individual attendee profiles.
- **Financial Monitoring** — Track payments, refunds, and coupon usage across your events.
- **Account Statistics** — Get real-time insights into your total registrations and account growth.

### How it works

1. Connect the Corsizio integration to your AI assistant.
2. Authorize using your Corsizio Secret API Key (found in Account Settings > Developer API).
3. Manage your event lifecycle through intuitive conversation.

### Who is this for?

- **Event Organizers** — Quickly check registration counts and attendee details on the go.
- **Instructors & Teachers** — Access class lists and student information directly via chat.
- **Business Admins** — Monitor event revenue and financial transactions efficiently.


## Available Tools (10)
- **get_account_stats**: Resolves total revenue, registration counts, and event performance metrics.

Retrieve high-level statistics for your Corsizio account
- **get_attendee_details**: Touches personal details, payment history, and event enrollment boundaries.

Get full registration profile for an attendee
- **get_event_details**: Touches event configuration, pricing, and registration boundary.

Get detailed information for a specific event
- **list_attendees**: Resolves attendee name, email, registration date, and payment status.

List all registered attendees for a specific event
- **list_coupons**: Resolves code names, discount amounts (percentage or fixed), and expiration constraints.

List all discount codes and coupons
- **list_events**: Resolves properties such as event ID, name, date, time, and current registration status.

List all events in your Corsizio account
- **list_instructors**: Resolves instructor names, contact info, and associated specialties.

List all instructors or teachers
- **list_locations**: Resolves location names, addresses, and capacity limits.

List physical or online locations for events
- **list_payments**: Resolves payment IDs, amounts, currencies, and associated event/attendee references.

List all payment transactions
- **list_refunds**: Resolves refund amount, original transaction reference, and processing date.

List all processed refunds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corsizio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events for the next month."

**🤖 AI Agent:**
> I've found 3 upcoming events: 'Digital Marketing Workshop' (May 12), 'Advanced Yoga Class' (May 15), and 'Photography Basics' (May 20). Would you like to see the registration counts for these?

---

**👤 You:**
> "How many people are registered for the 'Photography Basics' event?"

**🤖 AI Agent:**
> There are currently 18 people registered for 'Photography Basics'. The event capacity is 25, so there are 7 spots remaining. Should I list the attendee names?

---

**👤 You:**
> "Show me the total revenue generated from registrations this week."

**🤖 AI Agent:**
> This week, you've generated a total of $1,250 from 12 new registrations. Your most popular event was 'Advanced Yoga Class'. Would you like a breakdown of payments by day?


## ❓ FAQ

**Q: How do I get a Corsizio API Key?**
Log in to your Corsizio account, navigate to **Account Settings > Developer API**, and you will find your Secret API Key there.

**Q: Can I process refunds via chat?**
This integration currently provides read-only access to lists of payments and refunds for auditing purposes. Refund processing should be done via the Corsizio dashboard.

**Q: Is my data secure?**
Yes, the integration uses the official Corsizio API with your encrypted secret key. We do not store your attendee data on our servers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corsizio](https://vinkius.com/mcp/corsizio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corsizio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corsizio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corsizio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corsizio": {
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
