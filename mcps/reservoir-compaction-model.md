# Reservoir Compaction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-compaction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Quantifies reservoir deformation, subsidence, and compaction drive.

## Description
This MCP server provides specialized simulation tools to model the physical deformation of a reservoir as pore pressure declines. It allows AI agents to calculate vertical subsidence using `calculate_vertical_subsidence`, estimate energy contribution via `estimate_compaction_drive`, and predict flow degradation with `predict_permeability_loss`. It also offers a holistic view of the reservoir's mechanical state through `summarize_reservoir_impact`.


## Available Tools (4)
- **calculate_vertical_subsidence**: Calculates the total vertical movement of the reservoir top due to compaction
- **estimate_compaction_drive**: Determines the volumetric contribution of compaction to the reservoir's energy
- **predict_permeability_loss**: Predicts how much the ability to flow is degraded by the reduction in pore space
- **summarize_reservoir_impact**: Provides a holistic view of the reservoir's mechanical state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Compaction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the vertical subsidence for a reservoir with 0.0001 compressibility, 100m thickness, and 5MPa pressure change using uniaxial mode."

**🤖 AI Agent:**
> The total vertical subsidence is 0.005 meters.

---

**👤 You:**
> "What is the predicted permeability loss if initial permeability is 150mD, initial porosity is 0.25, and porosity reduction is 0.02?"

**🤖 AI Agent:**
> The final permeability is 132.4 mD, representing a 11.73% reduction.

---

**👤 You:**
> "Estimate the compaction drive for a reservoir with 0.2 porosity, 0.0001 compressibility, 10MPa pressure change, and 50m thickness."

**🤖 AI Agent:**
> The drive contribution ratio is 0.001 and the total expelled volume is 0.01 units.


## ❓ FAQ

**Q: What is the difference between uniaxial and hydrostatic compaction?**
Uniaxial compaction assumes deformation is restricted to the vertical axis, whereas hydrostatic compaction assumes isotropic deformation in all directions.

**Q: How can I see the total impact on the reservoir?**
You can use the `summarize_reservoir_impact` tool to get a combined report of subsidence, drive ratio, and permeability loss.

**Q: Does this model account for permeability reduction?**
Yes, the `predict_permeability_loss` tool calculates how much the flow capacity is degraded as pore space shrinks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-compaction-model](https://vinkius.com/en/ai-agent-connect/reservoir-compaction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Compaction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-compaction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Compaction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-compaction-model": {
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
