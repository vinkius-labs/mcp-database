# Envoy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/envoy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workplace operations via Envoy — register visitors, book desks and rooms, track deliveries, and monitor office capacity directly from any AI agent.

## Description
Connect your **Envoy** workplace account to any AI agent and take full control of your office management and visitor registration through natural conversation.

### What you can do

- **Visitor Orchestration** — Register expected arrivals and deliver QR code invites seamlessly while mapping NDA tracking and security compliance natively
- **Hot Desk Management** — List all available desks and reserve physical workspace elements by committing exact timing payloads directly into the organizational map
- **Meeting Room Control** — Identify bookable rooms and spaces, calculating maximal volumetric tracking and reporting integration limits securely
- **Logistical Tracking** — Monitor incoming deliveries and package states, extracting pickup receipts and bypassing front desk barriers flawlessly
- **Office Capacity Auditing** — Measure real-time occupancy metrics and compute active relational loads to ensure workplace compliance bounding
- **Employee Presence Monitoring** — Analyze specific HR identity connections fetching log trails to validate physical office sign-ins across any date range
- **Location Navigation** — Iterate through global office locations and workspaces to parse precise geographic configurations and maximum capacity limits

### How it works

1. Subscribe to this server
2. Enter your Envoy API Key (found in Envoy Console > Integrations > API)
3. Start managing your workplace operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Office Managers** — manage visitor lists and desk reservations without opening the Envoy dashboard
- **Executive Assistants** — pre-register guests and book meeting rooms using natural language
- **Logistics Teams** — monitor package deliveries and coordinate office sign-ins in real-time
- **Security Teams** — audit office capacity and verify employee presence through natural conversation


## Available Tools (10)
- **list_locations**: List all office locations managed in Envoy
- **list_visitors**: List all visitors checked in or expected at an Envoy location
- **pre_register_visitor**: Pre-register a visitor in Envoy
- **list_deliveries**: List all deliveries at an Envoy location
- **list_desks**: List all hot desks at an Envoy location
- **reserve_desk**: Reserve a hot desk in Envoy
- **cancel_desk_reservation**: Cancel an Envoy desk reservation
- **list_rooms**: List all bookable rooms/spaces at an Envoy location
- **get_employee_signins**: Get employee sign-in data for an Envoy location
- **get_capacity**: Get real-time capacity data for an Envoy location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Envoy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pre-register guest 'Jane Doe' (jane@example.com) for tomorrow at 10 AM"

**🤖 AI Agent:**
> Guest registered! I've scheduled Jane Doe's arrival at your office for tomorrow at 10:00 AM. A QR code invite and NDA link have been sent to her email. Would you like to reserve a meeting room for this time?

---

**👤 You:**
> "Reserve desk 'D-101' at the 'Main Office' for next Friday"

**🤖 AI Agent:**
> Desk reserved! You have successfully booked desk D-101 for next Friday. Your reservation is confirmed in the Envoy organizational map and will appear on your office dashboard.

---

**👤 You:**
> "What is the current occupancy at the London office?"

**🤖 AI Agent:**
> Checking London capacity... There are currently 45 people checked in out of a 100-person limit (45% occupancy). The office is currently within compliance boundaries.


## ❓ FAQ

**Q: Can my agent register a guest before they arrive at the office?**
Yes. Use the 'pre_register_visitor' tool. Provide the visitor's name, email, and expected arrival time. The agent will command the Envoy backend to schedule the arrival and deliver a QR code invite seamlessly.

**Q: How do I book a hot desk for a specific date via chat?**
Use the 'reserve_desk' tool. Provide the location ID, the specific desk ID, and the target date (YYYY-MM-DD). Your agent will claim the desk in the Envoy organizational map and update the spatial UI instantly.

**Q: Can I monitor real-time office capacity through the agent?**
Absolutely. Use the 'get_capacity' tool for a specific location. The agent computes active relational loads measuring exact occupancy metrics, providing workplace compliance data through natural conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/envoy](https://vinkius.com/mcp/envoy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Envoy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `envoy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Envoy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "envoy": {
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
