# Beam Design Simplified MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/beam-design-simplified)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate reinforced concrete beam parameters including steel area, bar selection, and shear reinforcement.

## Description
This MCP server provides a complete suite of structural engineering tools for reinforced concrete beam design using the Ultimate Strength Design (USD) method. It allows AI agents to perform critical calculations such as `calculate_flexural_design` to find required steel area, `select_reinforcement_bars` for practical rebar combinations, `calculate_shear_reinforcement` for stirrup spacing, and `verify_deflection_limit` to ensure serviceability. It acts as a bridge between structural engineering principles and AI-driven design workflows.


## Available Tools (4)
- **select_reinforcement_bars**: Suggests a practical combination of standard rebar diameters and quantities to meet the required steel area
- **verify_deflection_limit**: Checks if the beam's calculated deflection stays within acceptable serviceability limits
- **calculate_flexural_design**: Determines the required amount of longitudinal steel reinforcement needed to resist the bending moment
- **calculate_shear_reinforcement**: Determines if shear stirrups are required and calculates the necessary spacing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beam Design Simplified** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the flexural design for a beam with a 5m span, 20kN/m load, 30MPa concrete, 400MPa steel, 300mm width, 500mm height, 40mm cover, and 16mm bar diameter."

**🤖 AI Agent:**
> The required steel area is 850.5 mm² with an effective depth of 442 mm and a moment capacity of 125.4 kNm.

---

**👤 You:**
> "Suggest bar combinations for a required steel area of 1200 mm² using 12, 16, and 20mm bars in a 300mm wide beam with 30mm minimum spacing."

**🤖 AI Agent:**
> A practical combination is using 4 bars of 20mm diameter, providing 1256.6 mm² of steel area with 45mm spacing.

---

**👤 You:**
> "Check if a beam with 5mm deflection on a 5000mm span passes the serviceability limit."

**🤖 AI Agent:**
> Yes, the deflection of 5mm is well within the allowable limit for a 5000mm span.


## ❓ FAQ

**Q: What design method does this tool use?**
The tool uses the Ultimate Strength Design (USD) method, which is a standard approach in USA and European structural codes.

**Q: Can I check if my beam meets deflection limits?**
Yes, you can use the `verify_deflection_limit` tool to check if the calculated deflection stays within acceptable serviceability limits for a given span.

**Q: How does the tool suggest rebar combinations?**
The `select_reinforcement_bars` tool evaluates available bar diameters and quantities to satisfy the required steel area while respecting minimum spacing requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/beam-design-simplified](https://vinkius.com/ai-agent-connect/beam-design-simplified)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beam Design Simplified** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beam-design-simplified` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beam Design Simplified** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beam-design-simplified": {
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
