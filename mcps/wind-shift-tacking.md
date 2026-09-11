# Wind Shift Tacking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wind-shift-tacking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [navigation](../categories/navigation.md)

Calculate optimal tacking strategies and VMG impact during wind shifts.

## Description
This MCP server provides tactical sailing intelligence to maximize Velocity Made Good (VMG) during wind shifts. It allows AI agents to analyze wind direction changes and determine the most efficient path toward an upwind target. Using tools like `calculate_tack_decision` and `get_heading_adjustment`, agents can decide whether to stay on a current tack or perform a maneuver, while `evaluate_vmg_impact` quantifies the efficiency changes. It is designed for sailors and tactical analysts needing precise heading adjustments and shift viability assessments.


## Available Tools (4)
- **calculate_tack_decision**: Determines whether the boat should stay on its current tack or perform a tack based on an upcoming wind shift
- **check_shift_timing_viability**: Assesses if a wind shift is significant enough to warrant a tactical maneuver
- **evaluate_vmg_impact**: Quantifies the efficiency lost or gained due to a specific wind shift
- **get_heading_adjustment**: Calculates the specific new heading required to optimize the boat's position after a wind shift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wind Shift Tacking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I tack given a 10 degree clockwise wind shift?"

**🤖 AI Agent:**
> The optimal action is to tack to starboard to catch the lift and increase VMG.

---

**👤 You:**
> "What is my new heading after a 5 degree counter-clockwise shift?"

**🤖 AI Agent:**
> Your new optimal heading is 275 degrees.

---

**👤 You:**
> "Is a 3 degree shift worth a maneuver?"

**🤖 AI Agent:**
> No, the maneuver penalty exceeds the predicted VMG advantage for such a small shift.


## ❓ FAQ

**Q: How does this tool help with wind shifts?**
It uses `calculate_tack_decision` to determine if a shift warrants a maneuver and `get_heading_adjustment` to find the new optimal heading.

**Q: Can I calculate the efficiency loss of a maneuver?**
Yes, the `evaluate_vmg_impact` tool quantifies the efficiency gained or lost due to wind shifts.

**Q: What is VMG?**
VMG (Velocity Made Good) is the component of a boat's speed directed toward its intended upwind destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wind-shift-tacking](https://vinkius.com/en/ai-agent-connect/wind-shift-tacking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wind Shift Tacking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wind-shift-tacking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wind Shift Tacking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wind-shift-tacking": {
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
