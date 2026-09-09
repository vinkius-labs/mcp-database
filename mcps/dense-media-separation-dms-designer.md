# Dense Media Separation (DMS) Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dense-media-separation-dms-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design efficient DMS circuits by calculating equipment dimensions, media properties, and separation performance.

## Description
This MCP server provides specialized engineering tools for designing Dense Media Separation (DMS) circuits used in mineral processing. It allows users to calculate necessary equipment dimensions for cyclones or drums, determine optimal media properties including viscosity impact, and estimate separation efficiency and recovery rates. Use `optimize_circuit_design` to verify the feasibility of a complete design based on ore density, throughput, and target cut points.


## Available Tools (4)
- **calculate_equipment_dimensions**: Determines the necessary physical size of the separation vessel (cyclone or drum) to handle the specified ore flow
- **determine_media_properties**: Calculates the ideal media density and evaluates the impact of viscosity on the separation process
- **evaluate_separation_performance**: Estimates the efficiency and recovery capabilities of the proposed design
- **optimize_circuit_design**: Provides a high-level summary and optimization check for a full set of design parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dense Media Separation (DMS) Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What size cyclone do I need for 50 tph throughput with an ore density of 2.8 and media density of 2.5?"

**🤖 AI Agent:**
> For a throughput of 50 tph, the required cyclone will have a diameter of 450mm, a height of 1200mm, and a volume of 1.9m³.

---

**👤 You:**
> "Calculate the media properties for a sink-float density of 2.6 and ore density of 2.9 with a viscosity of 0.05."

**🤖 AI Agent:**
> The optimal media density is 2.65, with a stability index of 0.85 and a viscosity impact factor of 0.92.

---

**👤 You:**
> "Is a design with 100 tph throughput, 2.7 cut point, 3.0 ore density, and 2.6 media density feasible for a drum?"

**🤖 AI Agent:**
> Yes, the design is feasible. The recommended diameter is 2200mm with an estimated separation efficiency of 94%.


## ❓ FAQ

**Q: How do I size a cyclone for my ore flow?**
You can use the `calculate_equipment_dimensions` tool. Provide the throughput, ore density, media density, and specify 'cyclone' as the equipment type.

**Q: Can I check if my design is feasible?**
Yes, the `optimize_circuit_design` tool performs a high-level optimization check to verify if the media density and equipment dimensions support the target separation.

**Q: How is separation efficiency calculated?**
The `evaluate_separation_performance` tool estimates efficiency based on the density difference between the ore and the medium, as well as the media recovery rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dense-media-separation-dms-designer](https://vinkius.com/ai-agent-connect/dense-media-separation-dms-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dense Media Separation (DMS) Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dense-media-separation-dms-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dense Media Separation (DMS) Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dense-media-separation-dms-designer": {
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
