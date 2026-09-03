# Concrete Waffle Slab Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-waffle-slab-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design structural waffle slab systems, calculating geometry, reinforcement, and shear capacity.

## Description
This MCP server provides a complete suite of structural engineering tools for designing two-way ribbed concrete systems. It allows engineers to determine physical dimensions using `calculate_slab_geometry`, calculate necessary steel reinforcement with `calculate_reinforcement_requirements`, verify safety against punching failure via `verify_punching_shear_capacity`, and ensure serviceability using `check_deflection_limits`.


## Available Tools (4)
- **calculate_reinforcement_requirements**: Requires the geometry object from calculate_slab_geometry.

Calculates the necessary steel area for bending and crack control
- **calculate_slab_geometry**: Determines the physical dimensions of the ribs and the total slab thickness
- **check_deflection_limits**: Requires the geometry object from calculate_slab_geometry.

Evaluates if the designed slab meets serviceability requirements for deflection
- **verify_punching_shear_capacity**: Requires the geometry object from calculate_slab_geometry.

Checks if the slab-column interface can withstand the concentrated load without punching failure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Waffle Slab Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the geometry for a waffle slab with a 6m span, 10 kN/m² load, 500mm rib spacing, and 30 MPa concrete."

**🤖 AI Agent:**
> The slab will have a rib width of 150mm, a rib height of 350mm, and a total slab thickness of 400mm.

---

**👤 You:**
> "Check if a slab with 400mm thickness and 10 kN/m² load is safe against punching shear for a 300x300mm column."

**🤖 AI Agent:**
> The slab is safe; the calculated shear capacity exceeds the applied shear force.

---

**👤 You:**
> "What is the reinforcement needed for a 5m span, 12 kN/m² load, and fixed supports using the previously calculated geometry?"

**🤖 AI Agent:**
> The required reinforcement includes 450mm² of top slab steel, 320mm² of rib steel, and 150mm² of minimum shrinkage steel.


## ❓ FAQ

**Q: What parameters are needed for geometry calculation?**
To use `calculate_slab_geometry`, you need the span in meters, the design load in kN/m², the rib spacing in mm, and the concrete strength in MPa.

**Q: How do I check if my slab is safe from punching shear?**
You can use the `verify_punching_shear_capacity` tool by providing the slab geometry, the design load, and the dimensions of the supporting column.

**Q: Can I design for different support conditions?**
Yes, the tools support 'simply_supported', 'continuous', and 'fixed' conditions to accurately model moment distribution and deflection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-waffle-slab-designer](https://vinkius.com/ai-agent-connect/concrete-waffle-slab-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Waffle Slab Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-waffle-slab-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Waffle Slab Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-waffle-slab-designer": {
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
