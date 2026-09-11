# Thermal Recovery Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/thermal-recovery-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulate and optimize thermal enhanced oil recovery (EOR) projects.

## Description
This MCP server provides specialized engineering tools for designing thermal enhanced oil recovery (EOR) projects. It allows AI agents to calculate optimal steam injection rates using `calculate_steam_injection_rate`, design efficient well configurations with `design_well_pattern`, and predict total yield via `estimate_oil_recovery`. Additionally, it can quantify energy dissipation through `analyze_thermal_losses` to ensure project efficiency.


## Available Tools (4)
- **analyze_thermal_losses**: Quantifies the energy lost to the non-productive layers
- **calculate_steam_injection_rate**: Determines the optimal rate of steam injection required to maintain a stable thermal front
- **design_well_pattern**: Determines the optimal spatial configuration and distance between wells
- **estimate_oil_recovery**: Predicts the total volume of oil that can be successfully recovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thermal Recovery Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal steam injection rate for a reservoir with 50 cP viscosity, 20m thickness, and 2.0 thermal conductivity at 250 degrees?"

**🤖 AI Agent:**
> The optimal steam injection rate is 150.5 units per hour with an energy efficiency of 72%.

---

**👤 You:**
> "Design a five-spot well pattern for a 15m thick reservoir with 100 cP viscosity and a steam injection rate of 200."

**🤖 AI Agent:**
> The optimal pattern size is 45m with a well spacing of 31.8m using the five-spot configuration.

---

**👤 You:**
> "Estimate the oil recovery for a reservoir 500m deep, 30m thick, with a 100m pattern size, 80 cP viscosity, and 250 steam injection rate."

**🤖 AI Agent:**
> The expected oil recovery is 1,250,000 barrels with a recovery factor of 35% and an efficiency loss of 12%.


## ❓ FAQ

**Q: How do I calculate the required steam injection rate?**
You can use the `calculate_steam_injection_rate` tool by providing the oil viscosity, reservoir thickness, thermal conductivity, and your target temperature.

**Q: Can I predict the total oil recovery for my reservoir?**
Yes, the `estimate_oil_recovery` tool predicts the total volume of oil that can be successfully recovered based on reservoir depth, thickness, pattern size, and injection rate.

**Q: How does this tool handle heat loss to surrounding rock?**
The `analyze_thermal_losses` tool specifically quantifies energy lost to the overburden and underburden layers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/thermal-recovery-design](https://vinkius.com/en/ai-agent-connect/thermal-recovery-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thermal Recovery Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thermal-recovery-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thermal Recovery Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thermal-recovery-design": {
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
