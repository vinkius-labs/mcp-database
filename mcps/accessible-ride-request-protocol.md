# Accessible Ride Request Protocol MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-ride-request-protocol)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Transforms complex accessibility needs and provider constraints into actionable ride request packages.

## Description
This MCP server acts as a logistics engine for accessible transportation. It validates mobility equipment dimensions against vehicle constraints using `validate_equipment_fit` and generates complete documentation via `generate_ride_request`. It also creates customized pickup checklists with `build_handoff_checklist` and verifies emergency contact sequences with `verify_contingency_chain` to ensure safe, reliable transit for users with specific physical requirements.


## Available Tools (4)
- **build_handoff_checklist**: Create a customized checklist for the user or caregiver to ensure a smooth transition at the pickup point
- **validate_equipment_fit**: Determine if specific mobility equipment can physically fit into a specific vehicle type
- **generate_ride_request**: Validate all inputs against provider rules and generate the full suite of ride documentation
- **verify_contingency_chain**: Ensure the fallback contact sequence is logically sound and contains all necessary escalation data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Ride Request Protocol** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a ride request for a wheelchair user from 123 Maple St to 456 Oak Ave with specific ramp requirements."

**🤖 AI Agent:**
> Request Brief: Pickup at 123 Maple St, Destination 456 Oak Ave. Equipment: Manual Wheelchair (Width: 26in, Length: 38in). Driver must use high-capacity ramp. Confirmation: Does the vehicle have a minimum 26-inch doorway clearance? Handoff: Confirm driver is at the curb and has the ramp deployed.

---

**👤 You:**
> "Check if a 30-inch wide scooter fits in a vehicle with 28 inches of interior width."

**🤖 AI Agent:**
> The equipment is not compatible because the scooter width (30 inches) exceeds the vehicle's interior width clearance (28 inches).

---

**👤 You:**
> "Verify my emergency contact list: Alice (555-0101) and Bob (555-0102)."

**🤖 AI Agent:**
> The contingency chain is verified. Sequence: Alice, then Bob. Total contacts: 2.


## ❓ FAQ

**Q: How does the tool ensure equipment will fit in the vehicle?**
The `validate_equipment_fit` tool compares the physical dimensions and weight of the mobility aid against the specific interior clearances and ramp capacities of the vehicle.

**Q: What is included in the ride request package?**
The `generate_ride_request` tool produces a request brief for the driver, confirmation questions for the user, a handoff checklist, and a fallback contact sequence.

**Q: Can I customize the pickup instructions?**
Yes, the `build_handoff_checklist` tool creates a personalized sequence of actions based on your specific transfer preferences and communication needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-ride-request-protocol](https://vinkius.com/en/ai-agent-connect/accessible-ride-request-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Ride Request Protocol** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-ride-request-protocol` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Ride Request Protocol** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-ride-request-protocol": {
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
