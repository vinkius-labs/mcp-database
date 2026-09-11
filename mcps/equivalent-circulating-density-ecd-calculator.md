# Equivalent Circulating Density (ECD) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/equivalent-circulating-density-ecd-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Calculate ECD profiles, cuttings impact, and environmental adjustments for drilling fluids.

## Description
This MCP server provides critical drilling engineering calculations. It allows AI agents to determine the Equivalent Circulating Density (ECD) at specific depths using `calculate_ecd_profile`. It also assesses how rock fragments increase density via `calculate_cuttings_impact`, compares static and dynamic pressure states with `compare_static_dynamic_states`, and adjusts mud properties for temperature and pressure using `adjust_for_environment`.


## Available Tools (4)
- **adjust_for_environment**: Modify the baseline mud properties based on the thermal and pressure environment at depth
- **calculate_cuttings_impact**: Assess how the concentration of rock fragments in the annulus increases the effective density
- **calculate_ecd_profile**: Determine the ECD at various specific depths within the wellbore
- **compare_static_dynamic_states**: Provide a direct comparison between the pressure exerted when the pumps are off versus when they are on


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equivalent Circulating Density (ECD) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ECD profile for a mud weight of 10.5 ppg, flow rate of 500 gpm, hole diameter of 8.5 inches, pipe diameter of 5 inches, rheology of {viscosity: 25, yieldPoint: 15}, at depths 5000, 7000, and 10000 feet."

**🤖 AI Agent:**
> At 5000 ft, the ECD is 10.62 ppg. At 7000 ft, the ECD is 10.65 ppg. At 10000 ft, the ECD is 10.68 ppg.

---

**👤 You:**
> "What is the impact of 5% cuttings concentration on a 12.0 ppg mud with an annular velocity of 150 ft/min?"

**🤖 AI Agent:**
> The effective density is 12.45 ppg, resulting in a density increase of 0.45 ppg.

---

**👤 You:**
> "Compare static and dynamic pressure for a 11.0 ppg mud at 8000 ft with an annular pressure loss of 200 psi."

**🤖 AI Agent:**
> The static pressure is 4573 psi and the dynamic pressure is 4757 psi, with a pressure differential of 184 psi.


## ❓ FAQ

**Q: How can I calculate the ECD at different depths?**
You can use the `calculate_ecd_profile` tool by providing the mud weight, flow rate, hole and pipe diameters, rheology parameters, and the list of target depths.

**Q: Does this tool account for temperature changes?**
Yes, the `adjust_for_environment` tool allows you to modify baseline mud weight and viscosity based on local temperature and bottom hole pressure.

**Q: Can I see the difference between static and dynamic pressure?**
Yes, the `compare_static_dynamic_states` tool provides a direct comparison between static pressure and dynamic pressure including the differential.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/equivalent-circulating-density-ecd-calculator](https://vinkius.com/en/ai-agent-connect/equivalent-circulating-density-ecd-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equivalent Circulating Density (ECD) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equivalent-circulating-density-ecd-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equivalent Circulating Density (ECD) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equivalent-circulating-density-ecd-calculator": {
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
