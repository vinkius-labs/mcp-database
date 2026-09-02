# Basement Waterproofing Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/basement-waterproofing-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Technical tool for designing basement waterproofing systems, including membranes and drainage.

## Description
This MCP server provides specialized engineering tools to design comprehensive basement waterproofing systems. By analyzing hydrostatic pressure, soil permeability, and water table levels, it determines the optimal waterproofing strategy. Use `analyze_waterproofing_strategy` to decide between tanking or drainage approaches, `design_membrane_system` to select appropriate materials, `calculate_drainage_specs` for sump and pump requirements, and `evaluate_structural_integrity` to verify safety factors against hydrostatic loads.


## Available Tools (4)
- **calculate_drainage_specs**: Designs the physical drainage layer and sump components
- **design_membrane_system**: Specifies the appropriate membrane type and material properties
- **evaluate_structural_integrity**: Checks if the proposed design meets safety standards
- **analyze_waterproofing_strategy**: Determines whether the design should follow a tanking, drainage, or hybrid approach


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basement Waterproofing Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a waterproofing strategy for a 4m deep basement with a water table at 2m and high soil permeability."

**🤖 AI Agent:**
> The recommended strategy is a Hybrid approach due to the high permeability and active hydrostatic pressure from the water table being above the floor level.

---

**👤 You:**
> "What membrane should I use for a C35/45 concrete with aggressive chemical exposure?"

**🤖 AI Agent:**
> An Industrial grade HDPE membrane with a thickness of 3.5mm is recommended to provide high chemical resistance.

---

**👤 You:**
> "Calculate the drainage requirements for a site with 1e-5 m/s permeability and a 5m basement depth."

**🤖 AI Agent:**
> The required drainage layer thickness is 150mm, with a sump capacity of 500L and a pump flow rate of 2.5 Lps.


## ❓ FAQ

**Q: How do I decide between tanking and drainage?**
You should use the `analyze_waterproofing_strategy` tool. It evaluates soil permeability and water table levels to recommend a tanking (barrier) or drainage (relief) approach.

**Q: Can this tool verify if my concrete is strong enough?**
Yes, the `evaluate_structural_integrity` tool calculates the safety factor by comparing the applied hydrostatic load against the specified concrete grade.

**Q: What information is needed for drainage calculations?**
To use `calculate_drainage_specs`, you need to provide the soil permeability, basement depth, water table level, and the chosen strategy type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/basement-waterproofing-designer](https://vinkius.com/ai-agent-connect/basement-waterproofing-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basement Waterproofing Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basement-waterproofing-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basement Waterproofing Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basement-waterproofing-designer": {
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
