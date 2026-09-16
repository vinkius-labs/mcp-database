# Floating Roof Tank Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/floating-roof-tank-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Automated design of floating roof storage tanks following API 650 Appendix C standards.

## Description
This MCP server provides specialized engineering tools for designing floating roof storage tanks in compliance with API 650 Appendix C. It enables AI agents to perform critical calculations for roof architecture, seal selection, and environmental stability. Use `select_roof_type` to determine the best architecture, `calculate_seal_system` for containment requirements, `evaluate_environmental_stability` to assess wind and seismic risks, and `design_roof_drainage` to manage rainwater accumulation.


## Available Tools (4)
- **calculate_seal_system**: Identifies the necessary primary and secondary seal configurations
- **design_roof_drainage**: Determines the capacity and placement of roof drains to prevent weight accumulation
- **evaluate_environmental_stability**: Assesses the risk of roof tilting or submergence due to wind and seismic events
- **select_roof_type**: Determines the most appropriate floating roof architecture for a given tank configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floating Roof Tank Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend a roof type for a 30m diameter tank storing liquid with a density of 850 kg/m3 and a max wind speed of 40 m/s."

**🤖 AI Agent:**
> For a 30m diameter tank with a product density of 850 kg/m3, a pontoon roof is recommended with a stability margin of 1.45.

---

**👤 You:**
> "What seal system is needed for a 20m diameter tank with high volatility product using a pontoon roof?"

**🤖 AI Agent:**
> A high-performance mechanical seal system is required, featuring a primary liquid-tight seal and a secondary vapor seal with a total width of 0.6 meters.

---

**👤 You:**
> "Calculate the drainage requirements for a double-deck roof with a 25m diameter and 50mm/hr rainfall intensity."

**🤖 AI Agent:**
> The design requires 4 flexible hose drains with a total capacity of 120 liters per minute to prevent weight accumulation.


## ❓ FAQ

**Q: What standards does this server follow?**
All calculations and design recommendations are based on the API 650 Appendix C standards for floating roof tanks.

**Q: Can I use this for both pontoon and double-deck roofs?**
Yes, the `select_roof_type` tool evaluates both pontoon and double-deck configurations to find the optimal solution for your tank diameter and product density.

**Q: How does the server handle environmental risks?**
The `evaluate_environmental_stability` tool assesses the risk of tilting or submergence by analyzing wind loads and seismic acceleration against the roof's buoyancy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/floating-roof-tank-designer](https://vinkius.com/en/ai-agent-connect/floating-roof-tank-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floating Roof Tank Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `floating-roof-tank-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floating Roof Tank Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floating-roof-tank-designer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
