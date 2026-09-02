# Flare System Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/flare-system-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Sizing emergency relief flare systems using API 521 methodologies.

## Description
This MCP server provides specialized engineering tools for sizing emergency relief flare systems. It follows API 521 methodologies to calculate critical parameters including flare stack height, tip diameter, and safe radiation distances. Users can use `get_relief_profile` to analyze gas properties, `calculate_tip_diameter` to manage exit velocities, and `calculate_radiation_distance` to ensure safety limits are met. The `sizing_summary` tool orchestrates the full workflow to provide a complete stack height recommendation based on mass flow, gas composition, and wind speed.


## Available Tools (4)
- **calculate_tip_diameter**: Determines the optimal diameter of the flare tip to manage exit velocity
- **calculate_radiation_distance**: Finds the minimum distance from the flare tip required to meet a specific radiation safety limit
- **get_relief_profile**: Calculates the fundamental properties of the relief stream based on mass flow and composition
- **sizing_summary**: Performs the complete sizing orchestration to provide a final stack height recommendation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flare System Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the relief profile for a gas with 90% Methane and 10% Ethane at a mass flow of 5 kg/s."

**🤖 AI Agent:**
> The relief profile shows a total molecular weight of 17.2 and a heat of combustion of 50.1 MJ/kg.

---

**👤 You:**
> "What is the required tip diameter for a 10 kg/s mass flow with a max exit velocity of 0.5 m/s?"

**🤖 AI Agent:**
> The optimal tip diameter is 1.25 meters.

---

**👤 You:**
> "Provide a full sizing summary for a 20 kg/s relief load with 100% Methane, a 15 kW/m2 radiation limit, and 5 m/s wind speed."

**🤖 AI Agent:**
> The recommended stack height is 35 meters with a tip diameter of 0.8 meters to maintain a safe distance for personnel.


## ❓ FAQ

**Q: What engineering standard does this tool follow?**
The tool follows the API 521 methodology for pressure-relieving and depressuring systems.

**Q: How do I calculate the final stack height?**
You can use the `sizing_summary` tool, which orchestrates the diameter and radiation calculations to recommend a safe stack height.

**Q: Can I account for wind speed in radiation calculations?**
Yes, the `calculate_radiation_distance` tool accounts for flame tilt caused by ambient wind speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/flare-system-sizing](https://vinkius.com/ai-agent-connect/flare-system-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flare System Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flare-system-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flare System Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flare-system-sizing": {
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
