# Brushfire MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/brushfire)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage events and attendees via Brushfire — track registrations, check-in guests, and monitor orders directly from any AI agent.

## Description
Connect your **Brushfire** account to any AI agent and orchestrate your event management, ticketing, and attendee synchronization through natural conversation.

### What you can do

- **Event Oversight** — List all your managed events, retrieve detailed metadata, and monitor ticket types.
- **Attendee Management** — List all registered guests for specific events, retrieve detailed profiles, and update information.
- **Real-time Check-in** — Mark attendees as checked-in directly from your workspace to track attendance.
- **Order Tracking** — List and inspect all event orders and transaction histories.
- **Registration Coordination** — Access and verify ticket/registration types to ensure your event setup is correct.
- **Account Insights** — Retrieve core account and site information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Brushfire API Key and Client Version
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — quickly check registration counts or attendee details without manual dashboard work.
- **On-site Staff** — perform check-ins and verify guest information straight from their mobile agent.
- **Finance Teams** — monitor event orders and transaction statuses using natural language.


## Available Tools (16)
- **cancel_attendee**: Administrative only: it does not move money, so handle refunds elsewhere.
The attendee disappears from check-in lists, and it cannot be undone from this tool.

Cancel one attendee registration by attendee ID. No financial change is made — it only marks the registration cancelled
- **get_attendee**: It takes an attendee ID, not an email — if you only have an email, use find_attendee_by_email to get the ID.

Get full details of one attendee by ID: name, contact details, ticket type, ticket code, order reference and check-in state
- **get_event**: Use it once you already have the event ID from list_events.
Nothing back means the ID is wrong or the account cannot see that event.

Get full details of one event: name, schedule, venue, ticket types, status and configuration, by its event ID
- **get_order**: For questions like "what's on my order" or "did my payment go through". Takes the order ID — find it with list_orders if you only know the buyer's name or email.

Get full details of one order by ID: buyer information, attendee line items, ticket types, fees, taxes and payment state
- **list_attendees**: Get the session ID from list_sessions, not from the event. `search` matches names; paginate with `qty` and `skip`.
The ticket code (`Code`) in each row is what check_in_attendee needs — not the attendee ID.

List the attendees registered for one check-in session, with each attendee name, ID, ticket code and check-in status. Supports name search and pagination
- **list_ticket_types**: Use it to answer "what tickets does this event offer", or to get the `attendee_type_id` that update_attendee needs.
Only types currently on sale are listed.

List the attendee (ticket) types available for an event, including each type name, ID, price and remaining inventory
- **set_attendee_completed**: Takes the attendee ID and `completed` ("true"/"false").
This is not check-in: check_in_attendee records arrival, this records that the person finished (a course, a shift, a station).

Mark one attendee as completed (finished the event) or not completed, by attendee ID
- **archive_event**: Brushfire is the soft-delete here.
It is asynchronous: the request returns queued, and an email is sent once it is done.
Hard to reverse — confirm the event name with the user first, and only archive events that are already over.

Archive one event by ID. The event is queued for archiving and an email is sent on completion
- **check_in_attendee**: Takes the session ID (from list_sessions) and the ticket code (the `Code` field from get_attendee or list_attendees — not the attendee ID).
Use it at the door to mark someone arrived. If the result says verification is required, the attendee must confirm details with staff.

Check one attendee into a session using their ticket code, recording the check-in time. Returns the result, including whether verification is required
- **checkout_attendee**: Takes the session ID and the ticket code, like check_in_attendee.
Use it when someone was checked in by mistake or into the wrong session. Only works on attendees currently checked in.

Reverse a check-in: check one attendee back out of a session using their ticket code
- **find_attendee_by_email**: The fastest way to resolve "who is this person" when a guest only knows their email, and it yields the attendee ID that get_attendee, update_attendee and cancel_attendee need.
Nothing back means the email is not registered — check the spelling or ask for the email used at purchase.

Find attendees across all events by their email address, returning each match with name, event and attendee ID
- **list_events**: Starting point for most workflows: you need an event ID before listing sessions, ticket types or orders.
Filter with `search` (matches part of a name); paginate with `qty` and `skip`. Empty result means no match — drop the search term.

List the events managed in Brushfire, with the event name, ID, dates and status for each. Supports name search and pagination
- **list_orders**: Use it to find an order ID before fetching one in full, or to answer "who bought and what did they pay".
Pass an event ID to narrow the results; without it the list spans the whole account and can be long.

List ticket orders, with order ID, buyer, items, totals and payment status. Can be filtered to a single event
- **list_sessions**: Always call this before list_attendees or check_in_attendee: in Brushfire, attendees belong to a session, not to the event, so those tools take a session ID, not an event ID.
One event may hold many sessions (e.g. one per day). If several, pick the one the user means from its name and start time.

List the check-in sessions of an event, with each session name, ID, start time and attendance counts. Sessions are the scope for listing and checking in attendees
- **resend_order_confirmation**: The answer to "I never got my tickets" — resend instead of reading the order out. If you only know the buyer's email, find the order ID with list_orders first.
The email goes to the address on the order, not to any other address.

Resend the purchase confirmation email for one order, by order ID
- **update_attendee**: Requires cart ID, event ID and attendee ID. Only the fields you pass change.
Get a valid `attendee_type_id` from list_ticket_types. This tool cannot rename a person or change their email.

Update an attendee inside a cart: change the ticket type, move them to a group, override the price, apply a discount, or set an external reference code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brushfire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Brushfire."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming conferences: 'Summer Summit 2026' (ID: ev_1), 'Tech Workshop' (ID: ev_2), and 'Global Gala' (ID: ev_3).

---

**👤 You:**
> "Show the attendee list for 'Summer Summit 2026'."

**🤖 AI Agent:**
> Retrieving attendees for Summer Summit... I found 150 registered guests, including Alice Johnson (Checked-in) and Bob Smith (Pending). Would you like to find someone specific?

---

**👤 You:**
> "Check-in attendee with ID att_99283."

**🤖 AI Agent:**
> Attendee att_99283 has been successfully checked-in for the event. Their status is now marked as present in Brushfire.


## ❓ FAQ

**Q: Can I check-in an attendee using the agent?**
Yes! Use the `check_in_attendee` tool with the Attendee ID. Your agent will update the status in Brushfire instantly to mark the guest as present.

**Q: How do I see the list of all attendees for my event?**
Simply ask the agent to `list_attendees` and provide the Event ID. It will retrieve all the registered guests, including names and statuses, from your Brushfire account.

**Q: Does the integration allow updating attendee details?**
Yes. Use the `update_attendee` action and provide the Attendee ID along with the new name or email. The information will be synchronized with Brushfire immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/brushfire](https://vinkius.com/en/ai-agent-connect/brushfire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brushfire** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brushfire` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brushfire** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brushfire": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
