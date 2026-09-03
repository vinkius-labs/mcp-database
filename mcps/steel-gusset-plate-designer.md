# Steel Gusset Plate Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-gusset-plate-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design structural gusset plate connections using Whitmore section and block shear analysis.

## Description
This MCP server provides structural engineering tools to design gusset plate connections. It calculates required plate thickness to prevent buckling, determines physical dimensions using Whitmore section analysis, and specifies both bolt layouts and weld requirements. The tools account for eccentricity and interaction effects to ensure safe force transfer between brace members and supporting structures.


## Available Tools (4)
- **determine_plate_dimensions**: Calculates the necessary width and height of the gusset plate
- **calculate_plate_thickness**: Determines the minimum required thickness of the gusset plate
- **calculate_weld_requirements**: Determines the size and length of welds needed
- **design_bolt_layout**: Specifies the number, diameter, and spacing of bolts required


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Gusset Plate Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required thickness for a gusset plate with a 500kN brace force, 30 degree angle, S355 steel, and 50mm eccentricity."

**🤖 AI Agent:**
> The required plate thickness is 14.5 mm, with a capacity utilization of 0.82. Buckling is not critical at this thickness.

---

**👤 You:**
> "What are the dimensions needed for a gusset plate with 400kN force at a 45 degree angle and a 200mm beam width?"

**🤖 AI Agent:**
> The required plate dimensions are 250 mm in width and 320 mm in height, providing a Whitmore width of 185 mm.

---

**👤 You:**
> "Design a bolt layout for a 300kN force on a 12mm thick plate using S355 steel and 20mm bolts with 40mm edge distance."

**🤖 AI Agent:**
> The connection requires 4 bolts in a rectangular pattern with 75 mm spacing.


## ❓ FAQ

**Q: How does the tool handle plate buckling?**
The `calculate_plate_thickness` tool evaluates local buckling stability by considering the axial force, steel grade, and eccentricity to ensure the plate remains stable under load.

**Q: Can I design both bolted and welded connections?**
Yes. You can use `design_bolt_layout` to determine bolt patterns and spacing, or `calculate_weld_requirements` to find the necessary weld size and length.

**Q: What is the Whitmore section used for?**
The Whitmore section is used by `determine_plate_dimensions` to calculate the effective width of the gusset plate, ensuring the physical dimensions can safely carry the brace force.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-gusset-plate-designer](https://vinkius.com/ai-agent-connect/steel-gusset-plate-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Gusset Plate Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-gusset-plate-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Gusset Plate Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-gusset-plate-designer": {
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
