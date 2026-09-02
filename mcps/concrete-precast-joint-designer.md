# Concrete Precast Joint Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-precast-joint-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates structural dimensions for precast concrete connections.

## Description
This MCP server provides specialized engineering tools for designing structural connections between precast concrete elements. It calculates critical parameters such as dowel size, embedment length, weld size, and grout pad dimensions. Use `design_connection_parameters` to determine core structural dimensions, `validate_material_suitability` to check if material strengths meet load requirements, `get_connection_type_defaults` for geometric constraints, and `calculate_grout_area` to prevent material crushing.


## Available Tools (4)
- **calculate_grout_area**: Determines the necessary surface area for grout pads to avoid crushing the material
- **get_connection_type_defaults**: Provides the standard geometric constraints and default behavior for a specific connection type
- **validate_material_suitability**: Determines if the provided concrete and grout strengths are sufficient to support the intended forces
- **design_connection_parameters**: Calculates the core structural dimensions required for a specific precast joint configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Precast Joint Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the connection parameters for a BUTT_JOINT with 50kN tension, 30kN shear, and 20kN compression. The element is 500x500x1000mm, concrete is 35MPa, and grout is 40MPa."

**🤖 AI Agent:**
> The required dimensions for the BUTT_JOINT are: dowel size 20mm, embedment length 150mm, weld size 8mm, grout pad width 120mm, and grout pad length 120mm.

---

**👤 You:**
> "Is a 25MPa concrete strength sufficient for a 100kN compression force on a 100x100mm surface?"

**🤖 AI Agent:**
> No, the material is not suitable because the applied force exceeds the bearing capacity of the 25MPa concrete for that surface area.

---

**👤 You:**
> "What is the required grout area for a 45kN force on 40MPa grout?"

**🤖 AI Agent:**
> The required grout area is 1125 mm2.


## ❓ FAQ

**Q: How do I calculate the required dowel size?**
You can use the `design_connection_parameters` tool, providing the connection type, applied forces, element dimensions, and material strengths.

**Q: Can I account for construction phase loads?**
Yes, the `design_connection_parameters` tool allows you to provide `erectionForces` to ensure the design is safe during the assembly phase.

**Q: How is grout pad area determined?**
The `calculate_grout_area` tool determines the necessary surface area to ensure the applied force does not exceed the material's compressive strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-precast-joint-designer](https://vinkius.com/ai-agent-connect/concrete-precast-joint-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Precast Joint Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-precast-joint-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Precast Joint Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-precast-joint-designer": {
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
