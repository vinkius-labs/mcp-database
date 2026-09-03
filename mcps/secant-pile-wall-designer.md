# Secant Pile Wall Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/secant-pile-wall-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate structural and geotechnical parameters for secant pile retaining walls.

## Description
This MCP server provides specialized engineering tools for designing secant pile retaining walls. It allows for precise calculation of pile spacing using `calculate_wall_geometry`, determination of lateral earth and hydrostatic pressures via `analyze_soil_pressure`, calculation of required stability depth with `determine_embedment_depth`, and steel reinforcement design through `design_structural_reinforcement`. It supports both hard-soft and hard-hard pile configurations to ensure geotechnical stability and structural integrity.


## Available Tools (4)
- **calculate_wall_geometry**: Determines the physical arrangement and spacing of the piles based on diameter and overlap
- **design_structural_reinforcement**: Determines the necessary steel reinforcement to provide the required structural capacity
- **determine_embedment_depth**: Calculates the required depth of the piles below the excavation level to ensure geotechnical stability
- **analyze_soil_pressure**: Calculates the lateral earth pressures acting on the wall profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Secant Pile Wall Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pile spacing for a 600mm diameter pile with a 15% overlap in a hard-soft configuration."

**🤖 AI Agent:**
> The center-to-center spacing for the piles is 510mm.

---

**👤 You:**
> "What is the total lateral pressure for a 5m wall with a soil unit weight of 18 kN/m3, cohesion of 5 kPa, friction angle of 30 degrees, and a 2m water head?"

**🤖 AI Agent:**
> The total lateral pressure is 112.5 kPa.

---

**👤 You:**
> "Determine the reinforcement needed for a 600mm pile with a 150 kNm bending moment and 30 MPa concrete strength in a hard-soft setup."

**🤖 AI Agent:**
> The required steel area is 1250 mm2, with a suggested rebar diameter of 25mm.


## ❓ FAQ

**Q: What configurations are supported?**
The tool supports both hard-soft (Type A/B) and hard-hard (Type C) pile configurations.

**Q: How do I calculate the required depth for stability?**
You can use the `determine_embedment_depth` tool by providing the wall height, soil properties, and water head.

**Q: Can I design reinforcement for specific bending moments?**
Yes, the `design_structural_reinforcement` tool calculates the required steel area and suggested rebar diameter based on the bending moment and concrete strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/secant-pile-wall-designer](https://vinkius.com/ai-agent-connect/secant-pile-wall-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Secant Pile Wall Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `secant-pile-wall-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Secant Pile Wall Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "secant-pile-wall-designer": {
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
