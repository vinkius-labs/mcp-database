# Downwind Run Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/downwind-run-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Plan logistics for downwind runs, including distance, drift, and shuttle needs.

## Description
This MCP server provides essential logistics planning for downwind runs. It calculates total distance and lateral drift caused by wind, estimates duration using a fatigue factor, identifies strategic bailout points for safety, and determines shuttle vehicle requirements. Use `plan_run_route` to establish the path, `estimate_duration` to account for exhaustion, `identify_bailout_points` for safety planning, and `calculate_shuttle_needs` to coordinate vehicle logistics.


## Available Tools (4)
- **calculate_shuttle_needs**: Determines the vehicle logistics required to support the run
- **estimate_duration**: Calculates the total time required for the run, accounting for physical exhaustion
- **identify_bailout_points**: Determines strategic locations where a runner can safely stop and be retrieved
- **plan_run_route**: Calculates the primary physical logistics of the run including total distance and drift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Downwind Run Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the route for a run starting at 45.0, -75.0 and ending at 45.1, -75.1 with a wind direction of 90 degrees and speed of 10 km/h."

**🤖 AI Agent:**
> The total distance for the run is 15.2 km, with a calculated drift of 1.4 km.

---

**👤 You:**
> "How long will a 20km run take at 8 km/h with a fatigue factor of 1.2?"

**🤖 AI Agent:**
> The estimated duration is 3 hours.

---

**👤 You:**
> "How many shuttle trips are needed for a 50km run with 4 bailout points and a 5-hour duration?"

**🤖 AI Agent:**
> The logistics require 5 vehicle cycles covering a total shuttle distance of 65 km.


## ❓ FAQ

**Q: How does the tool account for wind?**
The `plan_run_route` tool calculates lateral drift based on the wind direction and the intended path.

**Q: What is a fatigue factor?**
It is a multiplier used in `estimate_duration` to adjust the expected time based on the runner's increasing exhaustion.

**Q: Can I plan for emergency exits?**
Yes, you can use `identify_bailout_points` to find safe locations to stop and be retrieved by a shuttle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/downwind-run-planner](https://vinkius.com/en/ai-agent-connect/downwind-run-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Downwind Run Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `downwind-run-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Downwind Run Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "downwind-run-planner": {
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
