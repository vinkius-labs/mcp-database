# Foundation Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foundation-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate total structural loads for columns and foundation beams.

## Description
This MCP server provides specialized tools for preliminary geotechnical analysis by calculating the vertical forces acting on foundations. Use `calculate_column_axial_load` to determine the total axial force at a column base, including permanent, variable, and self-weight components. Use `calculate_beam_linear_load` to find the distributed load along foundation beams based on spacing and floor count. Additionally, `get_structural_load_summary` provides an aggregated breakdown of all structural loads per unit area for your project profile.


## Available Tools (3)
- **calculate_beam_linear_load**: Calculates the linear load acting on a foundation beam
- **calculate_column_axial_load**: Calculates the total vertical force on a column base
- **get_structural_load_summary**: Provides a summary of structural loads for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foundation Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the axial load for a column with 5 kN/m² permanent load, 2 kN/m² variable load, 1 kN/m² self-weight per floor, 3 floors, and a 20 m² tributary area."

**🤖 AI Agent:**
> The total axial load for the column is 60.0 kN.

---

**👤 You:**
> "What is the linear load on a beam with 4 kN/m² permanent load, 1.5 kN/m² variable load, 0.5 kN/m self-weight, 2m spacing, and 5 floors?"

**🤖 AI Agent:**
> The distributed linear load for the foundation beam is 32.5 kN/m.

---

**👤 You:**
> "Provide a summary of loads for a building with 6 kN/m² permanent, 3 kN/m² variable, and 1.5 kN/m² self-weight per floor across 4 floors."

**🤖 AI Agent:**
> The structural load summary is: Total Permanent Load: 6.0 kN/m², Total Variable Load: 3.0 kN/m², and Total Self-Weight: 6.0 kN/m².


## ❓ FAQ

**Q: How is the column axial load calculated?**
The `calculate_column_axial_load` tool sums the permanent load, variable load, and the accumulated self-weight (self-weight per floor multiplied by the number of floors), all scaled by the provided tributary area.

**Q: What does the beam linear load represent?**
The `calculate_beam_linear_load` tool calculates the distributed weight (kN/m) acting along a foundation beam by combining permanent and variable loads from the slab area with the beam's own self-weight, multiplied by the number of floors.

**Q: Can I get a summary of all load types?**
Yes, use the `get_structural_load_summary` tool to receive an aggregated breakdown of total permanent, variable, and self-weight loads per unit area for your entire building footprint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foundation-load-calculator](https://vinkius.com/mcp/foundation-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foundation Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foundation-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foundation Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foundation-load-calculator": {
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
