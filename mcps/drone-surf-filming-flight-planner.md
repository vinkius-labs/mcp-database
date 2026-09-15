# Drone Surf Filming Flight Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/drone-surf-filming-flight-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [aviation](../categories/aviation.md)

Plan safe and efficient drone flight paths for capturing surf footage.

## Description
This MCP server provides specialized mission planning for drone operators capturing surf footage. It allows AI agents to generate precise waypoints using `plan_flight_path`, estimate battery consumption with `calculate_energy_needs` based on wind conditions, and ensure legal compliance via `validate_regulations`. Finally, it aggregates all data into a complete mission plan using `generate_mission_summary` to ensure flight safety and regulatory adherence.


## Available Tools (4)
- **calculate_energy_needs**: Estimates how much battery capacity is required to execute a specific flight path
- **generate_mission_summary**: Aggregates path, energy, and regulatory data into a final mission plan
- **plan_flight_path**: Generates a sequence of waypoints based on the desired filming shots and location
- **validate_regulations**: Checks if the proposed flight meets legal requirements for the specified region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drone Surf Filming Flight Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a flight path for a surf shoot at Pipeline, Hawaii."

**🤖 AI Agent:**
> The flight path has been generated with waypoints optimized for the wave break at Pipeline, ensuring all requested shots are covered.

---

**👤 You:**
> "Will my drone have enough battery for this flight in 15 knot winds?"

**🤖 AI Agent:**
> Based on the 15 knot wind speed, the estimated battery usage is 65%, leaving a safe 35% reserve.

---

**👤 You:**
> "Is it legal to fly at 150 feet in the USA?"

**🤖 AI Agent:**
> The flight is compliant with FAA regulations as it stays below the maximum altitude limit.


## ❓ FAQ

**Q: How does the tool ensure flight safety?**
The tool calculates a mandatory safety buffer by analyzing the flight path and wind conditions, ensuring sufficient battery remains for a safe return.

**Q: Can I check local drone laws?**
Yes, the `validate_regulations` tool checks the proposed flight against FAA and EASA requirements for the USA and Europe.

**Q: Does wind speed affect the planning?**
Yes, wind speed and direction are critical inputs for `calculate_energy_needs` to accurately predict battery usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/drone-surf-filming-flight-planner](https://vinkius.com/en/ai-agent-connect/drone-surf-filming-flight-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drone Surf Filming Flight Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drone-surf-filming-flight-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drone Surf Filming Flight Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drone-surf-filming-flight-planner": {
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
