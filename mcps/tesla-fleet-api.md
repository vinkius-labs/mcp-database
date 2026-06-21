# Tesla Fleet API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tesla-fleet-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Physical actuator proxy mapping explicitly native commands evaluating telemetry tracking active Tesla vehicles cleanly.

## Description
### What you can do

Take absolute proxy command over physically hosted Tesla vehicle hardware limits checking telemetries gracefully inside the Fleet Operator logic:

- **Track Hardware Executions natively** reading deep telemetry pulling explicitly GPS, Battery SoC, and Tire Pressures
- **Execute Physical Relays** actuating explicitly hardware limits bounding specific locks and interior HVAC bounds
- **Wake Sleeping Vehicles** directly triggering native relays catching cars in idle execution states parsing cleanly
- **Manage Fleet Commands** bounding honk and headlight mechanisms resolving completely natively safe locating structures

### ⚠️ CRITICAL WARNING: VEHICLE SLEEP STATE (HTTP 408)

**To conserve the high-voltage battery limits, Tesla vehicles physically sever their continuous network proxy when parked. If you execute a read (like `get_vehicle_data`) or a mechanical command (like `control_doors`) while the car is sleeping, the API will natively return `HTTP 408 Timeout`.**

The AI Agent MUST ALWAYS first invoke `wake_up_vehicle`, wait 10-15 seconds, and ONLY THEN route explicit subsequent logic telemetry proxies securely natively!

### How it works

1. **Define the Regional Proxy**, actively isolating endpoints correctly mapping your localized boundary (e.g. `na` for North America)
2. **Engage Fleet Tokens**, pulling `TESLA_FLEET_TOKEN` verifying cleanly limits inside the B2B configuration
3. **Map and execute hardware** navigating explicitly safely parsing latency errors bounding mechanically cleanly routing 

### Who is this for?

Specifically built for **Fleet Managers**, **Automotive Logistics Engineers**, and **Enterprise Operators** managing explicit Tesla vehicle matrices.


## Available Tools (8)
- **tesla_control_charge_port**: Call wake_up securely first executing correctly.

Engage explicitly the charging port relay actively isolating the power array bounds smoothly
- **tesla_control_doors**: Wake up first safely implicitly executing physical relays.

Actuate literal physical lock parameters securing or bounding native access inside the vehicle reliably
- **tesla_flash_lights**: Use tesla_wake_up_vehicle first resolving safely.

Trigger physical external headlight flash mechanisms securely bounding locating target implicitly
- **tesla_get_vehicle_data**: You MUST use tesla_wake_up_vehicle FIRST and wait before polling.

Extracts master telemetry matrices fetching explicitly SoC battery, Odometer, exact GPS coordinates, and vehicle internal temperatures
- **tesla_honk_horn**: Use tesla_wake_up_vehicle first bounding cleanly safely executing.

Actuate the physical hardware horn mechanism remotely triggering a loud alert locating the fleet proxy actively
- **tesla_list_vehicles**: Dumps explicit physical vehicle structs enumerating the exact active fleet array native list
- **tesla_trigger_climate**: Trigger explicit wake_up first parsing.

Engage explicitly the internal auto-conditioning climate system cleanly resolving temperature states before arrival
- **tesla_wake_up_vehicle**: Wait 10 seconds explicitly after calling this.

CRITICAL FIRST STEP: Trigger Explicit ignition matrices asserting the physical vehicle wakes from idle sleep states bounding actively over SaaS proxies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tesla Fleet API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check active fleet execution tracking natively extracting explicitly the battery SoC of vehicle XYZ safely resolving sleep delays initially."

**🤖 AI Agent:**
> Parsed logically evaluating native wake sequences (`wake_up_vehicle`) avoiding timeouts implicitly. After latency bounds resolved cleanly, (`get_vehicle_data`) extracted telemetry cleanly outputting 65% battery level appropriately safely routing inherently.

---

**👤 You:**
> "Actuate physical lock boundaries explicitly mapping the endpoints locking the doors inherently securely natively targeting 'car-aabbcc' dynamically."

**🤖 AI Agent:**
> Logical validation executed cleanly bounding constraints passing seamlessly checking actively wake states safely smoothly bounding locking explicit native parameters. (`control_doors`). Commands received explicitly locking.

---

**👤 You:**
> "Sound the explicit vehicle horn targeting proxy array bounds locating physical target effectively resolving native bounds gracefully mapping targets."

**🤖 AI Agent:**
> Validating native API timeouts smoothly tracking cleanly isolating `honk_horn` correctly asserting constraints parsing actively safely formatting physical responses perfectly cleanly.


## ❓ FAQ

**Q: Why does the API return HTTP 408 Timeout explicitly mapping bounds natively?**
Because the physical hardware is in Sleep Mode natively. Invoke `wake_up_vehicle` and strictly wait 10 seconds securely before parsing safely natively.

**Q: Can I explicitly control HVAC and climate parameters securely mapping local limits?**
Yes! Utilize `trigger_climate` exposing logic explicitly securely passing true/false bounds natively generating outputs cleanly.

**Q: What explicitly determines the API structural region explicitly mapping connections natively?**
The logical standard `TESLA_REGION` proxy explicitly parsing `na` (NA), `eu` (EU) bounds directly over the SDK native HTTP client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tesla-fleet-api](https://vinkius.com/mcp/tesla-fleet-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tesla Fleet API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tesla-fleet-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tesla Fleet API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tesla-fleet-api": {
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
