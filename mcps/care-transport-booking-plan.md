# Care Transport Booking Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-transport-booking-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Synchronizes medical appointments with specialized transit providers and mobility needs.

## Description
This MCP server acts as a coordination engine for medical logistics. It synchronizes medical appointments with specialized transit providers by accounting for mobility constraints, traveler availability, and budgetary limits. Use `plan_transport_logistics` to generate comprehensive logistical plans, `generate_pickup_timeline` for precise trip schedules, `create_rider_info_sheet` for driver summaries, and `get_backup_contacts` to identify secondary support if plans change.


## Available Tools (4)
- **create_rider_info_sheet**: Produces a concise summary for the driver and medical staff
- **generate_pickup_timeline**: Calculates the precise sequence of events for a single trip
- **get_backup_contacts**: Identifies secondary contacts if the primary transport plan fails
- **plan_transport_logistics**: Generates a comprehensive logistical plan including timelines and priorities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Transport Booking Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a transport for a wheelchair user for an appointment at 2024-10-15T14:00:00Z. Pickup is at 123 Maple St. Budget is $100. Providers: [{'id': 'p1', 'name': 'MedTrans', 'cost': 80, 'capabilities': ['wheelchair']}]."

**🤖 AI Agent:**
> The transport plan is ready. Priority 1: MedTrans ($80). Pickup is scheduled for 13:15:00Z to account for mobility lead time and travel buffers.

---

**👤 You:**
> "Generate a rider info sheet for John Doe, who needs assistance with walking, at 456 Oak Ave."

**🤖 AI Agent:**
> Rider Information Sheet: Name: John Doe. Location: 456 Oak Ave. Mobility Alert: Requires assistance with walking.

---

**👤 You:**
> "Calculate the pickup timeline for an appointment at 2024-11-01T09:00:00Z with a 30 minute travel duration and 15 minute buffer for limited mobility."

**🤖 AI Agent:**
> Departure time is 08:15:00Z. Arrival time is 08:45:00Z. A 15-minute buffer and mobility lead time have been applied.


## ❓ FAQ

**Q: How does the tool handle mobility constraints?**
The `plan_transport_logistics` tool evaluates provider capabilities against the specified mobility needs to ensure the vehicle and driver are appropriate for the rider.

**Q: Can I get a schedule for a specific trip?**
Yes, you can use `generate_pickup_timeline` to calculate exact departure and arrival times, including travel buffers and lead times.

**Q: What happens if the primary transport provider is unavailable?**
You can use `get_backup_contacts` to retrieve secondary or emergency contact information from the approved provider list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-transport-booking-plan](https://vinkius.com/en/ai-agent-connect/care-transport-booking-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Transport Booking Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-transport-booking-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Transport Booking Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-transport-booking-plan": {
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
