# Fracture Conductivity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fracture-conductivity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate hydraulic fracture conductivity, dimensionless conductivity (Fcd), and productivity gains while accounting for stress-induced proppant degradation.

## Description
This MCP server provides specialized engineering tools for hydraulic fracturing analysis. It allows AI agents to determine base fracture conductivity using proppant concentration, permeability, and width. Users can evaluate fracture effectiveness by calculating the dimensionless conductivity (Fcd) and estimate how reservoir stress affects proppant permeability via `estimate_stress_degradation`. Finally, it predicts the expected increase in well productivity based on conductivity targets. It is designed to bridge the gap between reservoir engineering data and AI-driven decision making.


## Available Tools (4)
- **calculate_dimensionless_conductivity**: Calculates the Fcd value to evaluate fracture effectiveness
- **calculate_fracture_conductivity**: Determines the base conductivity of the hydraulic fracture
- **estimate_stress_degradation**: Adjusts proppant permeability based on reservoir stress conditions
- **predict_productivity_gain**: Estimates the impact of the fracture on well performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fracture Conductivity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fracture conductivity for a width of 0.2 inches, proppant concentration of 5 lb/ft3, and permeability of 2000 darcy."

**🤖 AI Agent:**
> The calculated fracture conductivity is 400 darcy-inches.

---

**👤 You:**
> "How much will permeability degrade if effective stress is 5000 psi with a crush coefficient of 0.01 and initial permeability of 2000 darcy?"

**🤖 AI Agent:**
> The degraded permeability is 1500 darcy, representing a 25% loss.

---

**👤 You:**
> "Estimate the productivity gain if current Fcd is 2.0, target Fcd is 10.0, and base production is 500 bbl/d."

**🤖 AI Agent:**
> The expected production increase is 150 bbl/d, resulting in a productivity ratio of 1.3.


## ❓ FAQ

**Q: How do I calculate the base conductivity?**
Use the `calculate_fracture_conductivity` tool by providing the proppant concentration, initial proppant permeability, and the physical fracture width.

**Q: Can I account for proppant crushing?**
Yes, the `estimate_stress_degradation` tool allows you to adjust permeability based on effective stress and a specific material's crush coefficient.

**Q: What is Fcd?**
Fcd is the dimensionless conductivity, a ratio used to determine if a fracture is effectively conductive relative to the reservoir's permeability and half-length. You can calculate this using `calculate_dimensionless_conductivity`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fracture-conductivity-calculator](https://vinkius.com/en/ai-agent-connect/fracture-conductivity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fracture Conductivity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fracture-conductivity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fracture Conductivity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fracture-conductivity-calculator": {
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
