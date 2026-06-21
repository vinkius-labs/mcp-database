# OptimoRoute MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/optimoroute)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics-supply-chain](../categories/logistics-supply-chain.md)

Optimize delivery routes via OptimoRoute — create orders, run route planning, track driver GPS, and verify proof of delivery from any AI agent.

## Description
Connect your **OptimoRoute** account to any AI agent and orchestrate your entire route planning workflow from a single conversation.

### What you can do

- **Order Management** — Create delivery orders with addresses, time windows, and capacity constraints. Delete stale orders before they get routed
- **Route Optimization** — Queue route planning jobs with specific dates and driver sets, then check solver status or abort long-running computations
- **Route Downloads** — Download finalized manifest routes showing every optimized stop assigned to each driver
- **Scheduling Info** — Look up exactly when and where a specific order was scheduled within the optimized plan
- **Proof of Delivery** — Retrieve completion details including driver signatures, photos, and notes for verification
- **Live GPS Tracking** — Get real-time GPS coordinates for any driver in your fleet
- **Driver Configuration** — Update working hours, speed profiles, and load capacities for your drivers

### How it works

1. Subscribe to this server
2. Enter your OptimoRoute API Key
3. Start planning routes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics managers** — queue route optimizations and download manifests without opening the OptimoRoute dashboard
- **Dispatch teams** — create orders on the fly and track driver positions in real time during delivery windows
- **Operations analysts** — pull proof of delivery data and scheduling info for audit and compliance reporting


## Available Tools (10)
- **get_order_pod**: Retrieve the exact structural matching verifying Delivery success Proof
- **create_route_order**: Identify bounded routing spaces inside the Headless OptimoRoute platform
- **delete_stale_order**: Perform structural extraction of properties driving active Deletions
- **get_live_driver_gps**: Irreversibly vaporize explicit validations extracting Telemetry natively
- **download_manifest_routes**: Enumerate explicitly attached structured rules exporting active Drivers
- **check_planning_status**: Identify precise active arrays spanning native Asynchronous bounds
- **get_order_scheduling**: Dispatch an automated validation check routing explicit ETA models
- **queue_route_optimization**: Retrieve explicit Cloud logging tracing explicit solver logic
- **abort_route_planning**: Inspect deep internal arrays mitigating specific Time constraints
- **update_driver_shifts**: Provision a highly-available JSON Payload generating Truck constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OptimoRoute** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a delivery order for 200 Main St, Boston with a 2-hour time window from 9 AM to 11 AM."

**🤖 AI Agent:**
> Order ORD-4521 created successfully. Destination: 200 Main St, Boston, MA. Service time: 15 minutes. Time window: 09:00–11:00. The order is queued and ready for the next route optimization run. Want me to start a route optimization for today?

---

**👤 You:**
> "Start route optimization for tomorrow with drivers D1, D2, and D3."

**🤖 AI Agent:**
> Route optimization queued. Planning ID: PLN-7789. Solver is running with 3 drivers and 42 pending orders for April 1. Estimated completion: ~45 seconds. Want me to check the status in a moment?

---

**👤 You:**
> "Where is driver D2 right now?"

**🤖 AI Agent:**
> Driver D2 is currently at 42.3601, -71.0589 (near Faneuil Hall, Boston). Last ping: 12 seconds ago. Speed: 28 km/h. Currently en route to stop 4 of 8 (ETA: 5 minutes). Want me to pull the full route manifest for D2?


## ❓ FAQ

**Q: How long does route optimization take to complete?**
It depends on the number of orders and drivers. Small batches (under 100 stops) typically finish in under 30 seconds. Large-scale plans can take several minutes. The agent checks the planning status endpoint so you can monitor progress, and you can abort and capture the best partial solution at any time.

**Q: Can I verify if a delivery was actually completed with proof?**
Yes. The get_order_pod tool pulls completion details including driver-captured signatures, photos, and timestamped notes. This data comes directly from the OptimoRoute driver app and provides auditable proof of delivery for dispute resolution and compliance.

**Q: Can I update a driver's working hours and vehicle capacity on the fly?**
Yes. The update_driver_shifts tool lets you change working hours, speed profiles, and load capacities for any driver. Changes take effect on the next optimization run. Useful for adjusting schedules when a driver calls in sick or a vehicle needs to be swapped.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/optimoroute](https://vinkius.com/mcp/optimoroute)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OptimoRoute** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `optimoroute` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OptimoRoute** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "optimoroute": {
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
