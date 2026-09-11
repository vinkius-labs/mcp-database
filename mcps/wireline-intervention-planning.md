# Wireline Intervention Planning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wireline-intervention-planning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate mechanical loads, tool string configurations, and operational safety for wireline interventions.

## Description
This MCP server provides specialized engineering calculations for wireline operations in oil and gas wells. It allows AI agents to determine critical safety parameters including tension profiles, tool string viability, and pressure control compatibility. Use `get_tension_analysis` to model cable loads, `validate_toolstring_configuration` to ensure assembly safety, `check_pce_compatibility` to verify pressure equipment, and `calculate_depth_precision` to account for cable stretch.


## Available Tools (4)
- **calculate_depth_precision**: Estimates the potential error in tool depth positioning
- **check_pce_compatibility**: Ensures the selected Pressure Control Equipment is sufficient for the well conditions and tool string setup
- **get_tension_analysis**: Calculates the total tension profile of the wireline from the surface to the target depth
- **validate_toolstring_configuration**: Verifies if a proposed tool string assembly is physically and operationally viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wireline Intervention Planning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tension profile for a 5000m deployment with a 500kg tool string and 2kg/m cable in 1.1 density fluid."

**🤖 AI Agent:**
> The tension at 5000m is 12,450 kg, with a surface tension of 15,200 kg and an elastic stretch of 12.4 meters.

---

**👤 You:**
> "Is a tool string with components ['BHA_01', 'LOG_02'] safe if the max tension is 10000kg and total weight is 8500kg?"

**🤖 AI Agent:**
> Yes, the configuration is valid with a safety factor of 1.17.

---

**👤 You:**
> "Check if my PCE can handle 5000 psi for a 2.5 inch tool."

**🤖 AI Agent:**
> The equipment is compatible; the selected components support up to 6500 psi and accommodate the 2.5 inch diameter.


## ❓ FAQ

**Q: How does the tool calculate cable tension?**
The `get_tension_analysis` tool calculates tension by summing the buoyant weight of the tool string and the submerged weight of the cable at any given depth.

**Q: Can I verify if my pressure control equipment is safe?**
Yes, use `check_pce_compatibility` to compare your well pressure and tool diameter against the ratings of your available pressure control equipment.

**Q: How is depth error accounted for?**
The `calculate_depth_precision` tool estimates positioning error by analyzing the elastic stretch of the wireline under the calculated tension load.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wireline-intervention-planning](https://vinkius.com/en/ai-agent-connect/wireline-intervention-planning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wireline Intervention Planning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wireline-intervention-planning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wireline Intervention Planning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wireline-intervention-planning": {
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
