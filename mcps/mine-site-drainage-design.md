# Mine Site Drainage Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mine-site-drainage-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Hydrological engineering tools for designing mine site drainage, sizing infrastructure, and managing sediment risk.

## Description
This MCP server provides a suite of hydrological engineering tools to design safe and efficient drainage systems for mining operations. It allows AI agents to calculate peak runoff using `calculate_peak_flow`, determine ditch dimensions with `size_drainage_ditch`, and size culverts via `size_culvert`. Additionally, it includes capabilities to `evaluate_sediment_risk` and `design_diversion_path` to protect critical site assets from water ingress and erosion.


## Available Tools (5)
- **calculate_peak_flow**: Determines the maximum water volume expected during a design storm event
- **design_diversion_path**: Provides the necessary diversion requirements to protect specific site assets
- **evaluate_sediment_risk**: Assesses if the current drainage design provides sufficient sediment mitigation
- **size_culvert**: Determines the appropriate pipe or tunnel diameter for water crossing under infrastructure
- **size_drainage_ditch**: Calculates the required dimensions for open channels to safely contain peak water flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Site Drainage Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the peak flow for a 50 hectare area with 25 mm/hr rainfall and a 0.4 runoff coefficient."

**🤖 AI Agent:**
> The peak flow rate for the specified area is 50.0 m³/s.

---

**👤 You:**
> "What are the dimensions for a ditch with a peak flow of 2.5 m³/s, a 2% slope, and 1.5 m/s allowable velocity?"

**🤖 AI Agent:**
> The required ditch dimensions are a width of 3.5 meters and a depth of 1.8 meters.

---

**👤 You:**
> "Assess the sediment risk for a flow of 1.2 m³/s at a velocity of 0.8 m/s with a sediment load of 0.5 kg/m³."

**🤖 AI Agent:**
> The sediment risk level is Low, with an effectiveness score of 0.85.


## ❓ FAQ

**Q: How do I calculate the peak flow for a new catchment area?**
You can use the `calculate_peak_flow` tool by providing the rainfall intensity, the total catchment area in hectares, and the runoff coefficient.

**Q: Can this tool help with erosion control?**
Yes, you can use `evaluate_sediment_risk` to assess if your channel velocity and sediment load require further mitigation to prevent erosion.

**Q: How do I size a culvert for a haul road?**
Use the `size_culvert` tool with the peak flow rate, the culvert slope, and the maximum allowable headwater depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mine-site-drainage-design](https://vinkius.com/ai-agent-connect/mine-site-drainage-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Site Drainage Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-site-drainage-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Site Drainage Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-site-drainage-design": {
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
