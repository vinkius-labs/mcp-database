# TeamUp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teamup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Manage events, customers, coaches, memberships, and payments for your TeamUp-powered fitness studio through natural conversation.

## Description
Connect your **TeamUp** studio to any AI agent and manage your fitness business through natural conversation.

### What you can do

- **Events** — View scheduled classes and events with coaches, venues, and capacity
- **Event Types** — Browse class formats: CrossFit, Yoga, HIIT, Open Gym
- **Registrations** — Track who booked which class and check-in status
- **Customers** — Search members, view profiles, and track attendance
- **Memberships** — Browse all plans with pricing and billing frequency
- **Coaches** — List trainers with certifications and class assignments
- **Venues** — Manage training locations and room configurations
- **Payments** — Track revenue from memberships, drop-ins, and packages

### Who is this for?

- **Independent Studios** — Particularly popular in UK, EU, and Australia
- **CrossFit Boxes** — WOD scheduling, member tracking, and billing
- **Yoga Studios** — Class management and membership handling
- **Personal Trainers** — Client scheduling and payment tracking


## Available Tools (10)
- **list_events**: Filter by date range.

List scheduled classes/events
- **list_payments**: Includes amount, method, and member.

List payments and revenue
- **get_event**: Get event details
- **list_event_types**: Includes description, default duration, and default coach.

List class/event types
- **list_registrations**: Shows check-in status, waitlist position, and booking time.

List event registrations
- **search_customers**: Returns profile, active membership, visit count, and account balance.

Search members
- **get_customer**: Get member profile
- **list_memberships**: List membership plans
- **list_coaches**: List coaches and trainers
- **list_venues**: Includes address and capacity.

List training venues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TeamUp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's this week's class schedule?"

**🤖 AI Agent:**
> This week at your studio:

🏋️ **Monday**: CrossFit WOD 6:30 AM (Jake, 18/20), Yoga 7:00 PM (Sarah, 8/15)
🥊 **Tuesday**: Boxing 6:00 AM (Alex, FULL), HIIT 12:00 PM (Jake, 14/20)
🧘 **Wednesday**: Yoga Flow 9:00 AM (Sarah, 6/15), Open Gym 4:00 PM
🏋️ **Thursday**: CrossFit WOD 6:30 AM (Jake, 16/20), Mobility 7:00 PM (Ana, 5/12)
🥊 **Friday**: Friday Fight Club 5:30 PM (Alex, 19/20)

22 classes, Monday's Boxing is sold out!

---

**👤 You:**
> "Check the availability of exactly 'Conference Room A' for tomorrow afternoon."

**🤖 AI Agent:**
> Evaluating Teamup schedules ('get_events')...
'Conference Room A' (Sub-calendar ID: 301) is booked from 1:00 PM to 2:30 PM for 'Marketing Sync'. It is available fully from 2:30 PM until closing.

---

**👤 You:**
> "Schedule a new event 'Q1 Review Review' in the Executive Calendar for next Monday at 10 AM."

**🤖 AI Agent:**
> Executing `create_event` request on Teamup...
Event 'Q1 Review Review' successfully injected into the 'Executive Calendar'.
Date: Next Monday, 10:00 AM - 11:00 AM.
Event ID: `evt-8842`.


## ❓ FAQ

**Q: How do I get a TeamUp API key?**
Visit goteamup.com/developers to request developer API access. You'll receive an API key that must be passed in the X-Api-Key header with each request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teamup](https://vinkius.com/mcp/teamup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TeamUp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teamup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TeamUp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teamup": {
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
