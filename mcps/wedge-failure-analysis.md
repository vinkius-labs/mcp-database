# Wedge Failure Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wedge-failure-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze rock wedge stability, geometry, and support requirements.

## Description
This MCP server provides specialized engineering tools for evaluating the stability of rock wedges formed by intersecting discontinuities in slope faces. It allows for precise calculation of the Factor of Safety (FoS) by analyzing joint orientations, slope face angles, and friction. Users can evaluate environmental impacts such as water pressure and tension cracks, or calculate the necessary reinforcement using `calculate_required_support` to reach a target safety threshold. The toolset includes `analyze_wedge_stability` for primary metrics and `get_geometry_summary` for detailed spatial properties like intersection line length and wedge volume.


## Available Tools (4)
- **analyze_wedge_stability**: Determines the primary stability metrics for a specific wedge configuration
- **calculate_required_support**: Determines the necessary reinforcement needed to achieve a specific safety target
- **evaluate_environmental_impact**: Recalculates stability when considering water pressure, tension cracks, or additional loads
- **get_geometry_summary**: Provides a detailed breakdown of the spatial properties of the wedge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedge Failure Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the stability of a wedge with joint one at 120°/45°, joint two at 240°/40°, slope face at 0°/60°, friction angle of 30°, and weight of 500kN?"

**🤖 AI Agent:**
> The calculated Factor of Safety for this wedge configuration is 1.25, with an intersection dip of 35°.

---

**👤 You:**
> "How does adding 50kPa of water pressure affect my current stability?"

**🤖 AI Agent:**
> The addition of 50kPa water pressure reduces the adjusted Factor of Safety from 1.25 to 0.95, indicating potential instability.

---

**👤 You:**
> "What support is required to reach a target FoS of 1.5 given my current stability?"

**🤖 AI Agent:**
> To reach a target FoS of 1.5, a required support force of 120kN is needed, using grouted anchors.


## ❓ FAQ

**Q: How do I calculate the stability of a specific rock wedge?**
You can use the `analyze_wedge_stability` tool by providing the dip directions and angles for both joints and the slope face, along with the friction angle and wedge weight.

**Q: Can I account for water pressure in my stability analysis?**
Yes, use the `evaluate_environmental_impact` tool to recalculate the Factor of Safety while considering water pressure, tension cracks, and surcharge loads.

**Q: How much support is needed to reach a target Factor of Safety?**
The `calculate_required_support` tool determines the necessary reinforcement force and recommended bolt type to achieve your specific target FoS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wedge-failure-analysis](https://vinkius.com/ai-agent-connect/wedge-failure-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedge Failure Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedge-failure-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedge Failure Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedge-failure-analysis": {
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
