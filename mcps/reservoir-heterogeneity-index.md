# Reservoir Heterogeneity Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-heterogeneity-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Quantify reservoir heterogeneity using Dykstra-Parsons and Lorenz coefficients.

## Description
This MCP server provides specialized tools for quantifying reservoir heterogeneity to improve flow modeling and completion design accuracy. It allows AI agents to calculate the Dykstra-Parsons coefficient for permeability variation, determine the Lorenz coefficient for flow non-uniformity, evaluate anisotropy impact via vertical and horizontal permeability ratios, and classify distinct flow units based on hydraulic properties. By connecting to Vinkius Edge, these tools enable precise reservoir characterization through your preferred AI client like Cursor or Claude Desktop.


## Available Tools (4)
- **assess_anisotropy_impact**: Evaluates how vertical and horizontal permeability ratios affect the reservoir's overall heterogeneity
- **calculate_dykstra_parsons**: Calculates the Dykstra-Parsons coefficient to quantify permeability variation across layers
- **calculate_lorenz_coefficient**: Quantifies the degree of non-uniformity in flow using the Lorenz coefficient
- **classify_flow_units**: Groups reservoir layers into distinct flow units based on hydraulic properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Heterogeneity Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Dykstra-Parsons coefficient for permeability values [10, 50, 100, 200] and porosity values [0.2, 0.25, 0.22, 0.28]."

**🤖 AI Agent:**
> The calculated Dykstra-Parsons coefficient is 0.52, which indicates moderate heterogeneity.

---

**👤 You:**
> "What is the anisotropy impact if horizontal permeability is 100 mD and vertical permeability is 10 mD?"

**🤖 AI Agent:**
> The anisotropy ratio is 0.1, indicating significant vertical flow impedance due to the permeability ratio.

---

**👤 You:**
> "Determine the Lorenz coefficient for permeability [5, 10, 15, 20] and porosity [0.1, 0.12, 0.15, 0.18]."

**🤖 AI Agent:**
> The Lorenz coefficient is 0.12, suggesting a relatively uniform flow distribution.


## ❓ FAQ

**Q: How can I calculate permeability variation?**
You can use the `calculate_dykstra_parsons` tool by providing an array of permeability and porosity values.

**Q: What is the purpose of the Lorenz coefficient tool?**
The `calculate_lorenz_coefficient` tool quantifies the degree of non-uniformity in fluid flow within the reservoir.

**Q: Can I group reservoir layers into specific units?**
Yes, the `classify_flow_units` tool groups layers into distinct flow units based on their hydraulic properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-heterogeneity-index](https://vinkius.com/en/ai-agent-connect/reservoir-heterogeneity-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Heterogeneity Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-heterogeneity-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Heterogeneity Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-heterogeneity-index": {
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
