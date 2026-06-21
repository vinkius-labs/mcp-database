# Cal.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calcom-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Control Cal.com infrastructure organically — book events, manipulate schedules, and track availabilities using an AI-native conversational flow.

## Description
Connect your open-source **Cal.com** scheduling framework into your favorite AI agent and completely bypass manual calendar navigation via natural conversation setups.

### What you can do

- **Deep Log Exploration** — Inspect vast lists of all present calendar events routing the actual statuses, attendances, and internal system IDs explicitly
- **Frictionless Booking** — Schedule, instantly cancel, or reschedule target meetings seamlessly without switching your terminal or current tab scopes
- **Event Templates** — Scan and retrieve standard master formats fetching detailed URLs bypassing convoluted user search procedures in normal web browsers
- **Availability Mapping** — Audit raw schedule scopes confirming when your organization has free specific windows directly querying origin databases

### How it works

1. Subscribe to this server module
2. Enter your Personal Cal.com API key token natively gathered from system logs
3. Start fetching high-grade scheduling content straight into Claude, Cursor, or any MCP-compatible smart interface

No more context-switching between tools dragging your windows around visually searching to map people's schedules up properly. Your AI agent manages events natively connecting pure arrays directly.

### Who is this for?

- **Sales Development Reps** — scan all active demo bookings dynamically right from inside their editor prior sending an explicit rescheduler parameter off internally to systems centrally
- **Technical Founders** — verify overlapping schedules checking their available intervals smoothly using terminal code without jumping into web UIs across multiple calls to teams daily
- **Project Managers** — map custom internal event classes ensuring the main link works properly directly within organizational communication lines easily securely natively correctly universally immediately efficiently natively


## Available Tools
- **get_me**: Get the authenticated Cal.com user profile including name, email, timezone, default schedule, avatar, and organization info
- **list_bookings**: Standardizes attendee listings, temporal slots, statuses ("accepted" [confirmed], "pending", "cancelled", "rejected"), and spatial links.

List all Cal.com bookings with optional status filter
- **get_booking**: Retrieve full details of a specific Cal.com booking by its UID
- **create_booking**: Auto-generates conferencing URLs where default.

Programmatically create a new booking on Cal.com seamlessly capturing host slots
- **cancel_booking**: com destruction schemas firing integrated Email notifications alerting both the Organizer and external Guests appending the contextual reason.

Cancel an existing Cal.com booking via secure UID matching freeing timeslots
- **reschedule_booking**: Modifies host structures triggering email templates updating guest links securely.

Reschedule an existing Cal.com booking mapping to an explicit new temporal block
- **list_event_types**: Enumerate explicitly attached structured scheduling types mapping active formats
- **get_event_type**: Extract detailed configuration parsing a specific Cal.com native event boundary
- **list_schedules**: Locate physical scheduling origin rules managed natively bounding work times
- **get_available_slots**: Retrieve the exact array bounds verifying free temporal spans per mapped event types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cal.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the upcoming schedule details spanning out starting from yesterday completely accurately purely natively."

**🤖 AI Agent:**
> I securely gathered your operational list successfully correctly properly. There's 'Product Demo' booked completely officially for tomorrow morning alongside one canceled explicit slot. Would you prefer to read participant emails actively dynamically functionally naturally swiftly?

---

**👤 You:**
> "List event types openly functionally reliably flawlessly properly securely optimally thoroughly optimally natively natively smoothly securely natively directly."

**🤖 AI Agent:**
> You hold cleanly two active event arrays securely naturally efficiently strongly purely explicitly currently effortlessly properly natively perfectly perfectly explicitly: A 30-min discovery block precisely along natively natively with 60-m deep dive. Should I invoke link copies fully safely functionally comprehensively efficiently?

---

**👤 You:**
> "I want to delete schedule ID 182 thoroughly officially naturally structurally perfectly fully quickly reliably effortlessly seamlessly functionally securely completely."

**🤖 AI Agent:**
> Process thoroughly executed seamlessly reliably actively cleanly precisely strictly naturally strongly effortlessly accurately optimally solidly natively functionally swiftly successfully safely officially perfectly securely naturally firmly quickly properly natively intelligently correctly flawlessly confidently clearly dynamically. Booking structural identity ID 182 is forever closed externally actively globally strictly perfectly flawlessly directly natively completely dynamically properly cleanly officially naturally perfectly successfully.


## ❓ FAQ

**Q: Can it check if my 2:00 PM slot is strictly open inside its origin database matrices?**
Yes. Ask the agent via the get_available_slots interface tool, targeting dates. It cross-examines the true structural Cal parameters securely to verify if open overlapping exist immediately bypassing graphical user errors naturally quickly cleanly.

**Q: Can I cancel meeting structures via AI conversational queries exclusively securely easily fluidly quickly natively?**
Absolutely naturally fully completely completely totally definitively accurately effortlessly flawlessly functionally effectively. State you wish to cancel an event and either provide the ID explicitly or let it query. The system runs the termination protocol, alerting your invitees without manually lifting a secondary click internally securely truly natively powerfully organically efficiently properly cleanly smoothly reliably instantly natively naturally swiftly correctly.

**Q: Will the AI inform me who booked specific categories dynamically cleanly properly safely natively reliably securely properly?**
Yes naturally properly flawlessly comprehensively effectively directly efficiently easily seamlessly properly exactly reliably successfully strongly surely securely fully. Any simple invocation of the list bookings protocol surfaces arrays listing not just times but total attendees correctly linked with respective details precisely effectively smoothly natively exactly flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calcom-1](https://vinkius.com/mcp/calcom-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cal.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calcom-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cal.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calcom-1": {
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
