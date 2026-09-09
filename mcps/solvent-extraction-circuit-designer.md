# Solvent Extraction Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/solvent-extraction-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mining](../categories/mining.md)

Design copper or uranium solvent extraction circuits by calculating stages, equipment sizing, and reagent loading.

## Description
This MCP server provides specialized hydrometallurgical tools for designing solvent extraction (SX) circuits. It allows engineers to determine the minimum number of stages required using `calculate_stage_requirement`, size physical equipment with `size_mixer_settler`, and verify reagent capacity with `evaluate_reagent_loading`. It also includes `optimize_circuit_parameters` to balance equipment volume against recovery targets. The tools help manage critical factors like O:A ratios, throughput, and crud formation to ensure efficient metal recovery.


## Available Tools (4)
- **calculate_stage_requirement**: Determines the minimum number of extraction stages required to achieve a target metal recovery
- **evaluate_reagent_loading**: Assesses whether the chosen reagent concentration can support the target metal load
- **optimize_circuit_parameters**: Suggests adjustments to the O:A ratio or stages to improve efficiency
- **size_mixer_settler**: Calculates the physical dimensions (volume and area) required for the extraction units


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solvent Extraction Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many stages do I need for a 95% recovery of copper with a 0.5 O:A ratio and this isotherm: {"0.1": "0.05", "0.5": "0.3", "1.0": "0.7"}?"

**🤖 AI Agent:**
> To achieve 95% recovery with the provided isotherm and an O:A ratio of 0.5, 4 stages are required.

---

**👤 You:**
> "Calculate the mixer-settler dimensions for a throughput of 100 m3/h, O:A ratio of 1.2, residence time of 5 minutes, and a crud factor of 1.2."

**🤖 AI Agent:**
> The required equipment dimensions are: Mixer Volume: 120 m3, Settler Area: 450 m2, Mixer Diameter: 4.2 m, Settler Width: 15 m, and Settler Length: 30 m.

---

**👤 You:**
> "Is my reagent overloaded? Metal concentration is 5 g/L, throughput is 50 m3/h, reagent concentration is 0.1 M, and O:A ratio is 1.0."

**🤖 AI Agent:**
> The current loading is 85%, which is within the capacity limits.


## ❓ FAQ

**Q: How do I determine the number of stages needed?**
You can use the `calculate_stage_requirement` tool by providing the metal concentration, target recovery, the extraction isotherm, and the O:A ratio.

**Q: Can I account for impurities like crud?**
Yes, the `size_mixer_settler` tool includes a `crudFactor` parameter to adjust the required settler area for impurity buildup.

**Q: How do I check if my reagent is sufficient?**
Use the `evaluate_reagent_loading` tool to check if the reagent concentration can support the target metal load based on throughput and O:A ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/solvent-extraction-circuit-designer](https://vinkius.com/ai-agent-connect/solvent-extraction-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solvent Extraction Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solvent-extraction-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solvent Extraction Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solvent-extraction-circuit-designer": {
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
