# Fin Area Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fin-area-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Calculate optimal surfboard fin area and dimensions based on rider mass and wave energy.

## Description
This MCP server provides precise hydrodynamic calculations for surfboard designers and surfers. Use `calculate_total_required_area` to determine the aggregate surface area needed for a specific riding scenario. Once the total area is known, use `get_fin_dimensions` to find the specific height and width for each fin in a set. You can also use `calculate_fin_aspect_ratios` to evaluate performance characteristics like speed versus control, or `validate_setup_suitability` to ensure the fin setup is appropriate for the surfer's weight and board type.


## Available Tools (4)
- **calculate_total_required_area**: Determines the aggregate fin surface area needed for a specific riding scenario
- **get_fin_dimensions**: Calculates the specific height and width for each individual fin in a set
- **validate_setup_suitability**: Checks if a calculated fin setup is appropriate for a specific surfer and board combination
- **calculate_fin_aspect_ratios**: Provides the aspect ratio for each fin in a set to evaluate performance characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fin Area Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total fin area needed for an 80kg surfer on a 6ft board with medium wave power?"

**🤖 AI Agent:**
> The total required fin area for an 80kg surfer on a 6ft board with medium wave power is 450 cm2.

---

**👤 You:**
> "Give me the dimensions for a 3-fin thruster setup with a total area of 450 cm2."

**🤖 AI Agent:**
> For a thruster setup with 450 cm2, the dimensions are: Side Fin 1: height 12cm, width 5cm; Side Fin 2: height 12cm, width 5cm; Center Fin: height 14cm, width 6cm.

---

**👤 You:**
> "What is the aspect ratio for a fin that is 15cm high and 5cm wide?"

**🤖 AI Agent:**
> The aspect ratio for a fin with a height of 15cm and a width of 5cm is 3.0.


## ❓ FAQ

**Q: How do I determine the total fin area needed?**
You can use the `calculate_total_required_area` tool by providing the surfer's weight, the board length, and the wave power level.

**Q: Can I calculate dimensions for different fin setups?**
Yes, the `get_fin_dimensions` tool allows you to specify the template type (like thruster or quad) and the number of fins to get specific height and width measurements.

**Q: How do I know if my fin setup is safe for my weight?**
The `validate_setup_suitability` tool checks if the calculated area provides enough control for your specific weight and chosen template.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fin-area-calculator](https://vinkius.com/en/ai-agent-connect/fin-area-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fin Area Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fin-area-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fin Area Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fin-area-calculator": {
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
