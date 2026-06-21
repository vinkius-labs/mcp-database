# Momence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/momence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage sessions, members, teachers, memberships, and bookings for your Momence-powered fitness or yoga studio through natural conversation.

## Description
Connect your **Momence** studio to any AI agent and manage your fitness business through natural conversation.

### What you can do

- **Sessions** — View upcoming classes with teacher, capacity, waitlist, and streaming links
- **Members** — Search member database, view credits, tags, and attendance history
- **Teachers** — List instructors with bios, specialties, and class assignments
- **Memberships** — Browse plans: unlimited, class packs, intro offers, trials
- **Bookings** — Track who booked which session, check-in and waitlist status
- **Locations** — Manage multi-location studios with rooms and timezone
- **Products** — View retail items, digital content, and merchandise

### Who is this for?

- **Modern Yoga & Pilates Studios** — Momence is the fastest-growing studio platform, replacing Mindbody at independent studios
- **Boutique Fitness Owners** — Real-time class fill rates, member insights, and revenue tracking
- **Multi-Location Operators** — Consolidated view across all locations
- **Instructors** — Quick access to class rosters and member preferences


## Available Tools
- **list_sessions**: Filter by date range.

List scheduled sessions
- **list_products**: List products/retail
- **get_session**: Get session details
- **list_session_types**: with description, default duration, and default teacher.

List class types
- **search_members**: Returns profile, active memberships, credits, and visit history.

Search studio members
- **get_member**: Get member profile
- **list_memberships**: List membership plans
- **list_bookings**: List session bookings
- **list_teachers**: List teachers/instructors
- **list_locations**: List studio locations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Momence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How full are tomorrow's yoga classes?"

**🤖 AI Agent:**
> Tomorrow's yoga session fill rates:

🧘 7:00 AM **Sunrise Vinyasa** — 18/22 (82%) with Sarah ☀️
🧘 9:30 AM **Gentle Flow** — 8/18 (44%) with Ana
🧘 12:00 PM **Power Yoga** — FULL (waitlist: 3) with Jake 🔥
🧘 5:30 PM **Yin Restore** — 11/15 (73%) with Maria
🧘 7:00 PM **Hot Yoga** — 14/20 (70%) with Alex (online stream available)

Power Yoga is sold out! Yin Restore still has 4 spots — good candidate for a marketing push.

---

**👤 You:**
> "List the upcoming classes for instructor Sarah."

**🤖 AI Agent:**
> Sarah is scheduled to teach 'Sunrise Vinyasa' tomorrow at 7:00 AM, 'Core Pilates' on Thursday at 5:30 PM, and a special 'Yoga Retreat Workshop' this Saturday from 10:00 AM to 1:00 PM.

---

**👤 You:**
> "How many active members are on the Unlimited Monthly plan?"

**🤖 AI Agent:**
> You currently have 342 active members on the Unlimited Monthly plan. This represents a 5% increase from last month, largely driven by the recent introductory trial conversions.


## ❓ FAQ

**Q: What is Momence?**
Momence is a next-generation studio management platform used by thousands of yoga, pilates, barre, and boutique fitness studios worldwide. It's known for its modern UX, powerful API, and rapid innovation — many studios are migrating from Mindbody to Momence.

**Q: Does it support the Host API and Member API?**
This server uses the **Host API**, which provides access to all business management functions: sessions, members, bookings, memberships, teachers, and products. The Host API is the recommended choice for AI agents managing studio operations.

**Q: Can it process payments for memberships?**
While it can query membership details and pricing, actual payment processing and checkout must be handled through Momence's secure payment gateway for compliance reasons.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/momence](https://vinkius.com/mcp/momence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Momence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `momence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Momence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "momence": {
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
