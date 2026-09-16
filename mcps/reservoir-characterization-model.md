# Reservoir Characterization Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-characterization-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Analyzes petrophysical data to characterize reservoir properties and flow units.

## Description
This MCP server provides advanced analytical tools for petrophysical reservoir characterization. It transforms raw core and log data into actionable insights by calculating property distributions, assessing spatial heterogeneity, and identifying distinct flow units. Use `analyze_property_statistics` for high-level summaries, `evaluate_heterogeneity` to quantify spatial complexity, `identify_flow_units` to segment the reservoir, and `calculate_permeability_trends` to determine directional flow characteristics.


## Available Tools (4)
- **analyze_property_statistics**: Provides a high-level statistical summary of the basic petrophysical properties
- **calculate_permeability_trends**: Determines the directional flow characteristics of the reservoir
- **evaluate_heterogeneity**: Quantifies the complexity and spatial variation of the reservoir
- **identify_flow_units**: Segments the reservoir into distinct zones that function as unified fluid conduits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Characterization Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you provide a statistical summary for these porosity and permeability values? Porosity: [0.15, 0.18, 0.22], Permeability: [10, 15, 25], Saturation: [0.8, 0.75, 0.7]"

**🤖 AI Agent:**
> The mean porosity is 0.183, mean permeability is 16.67, and mean saturation is 0.75.

---

**👤 You:**
> "What is the permeability ratio if horizontal permeability is 50 mD and vertical permeability is 10 mD?"

**🤖 AI Agent:**
> The permeability ratio is 0.2, indicating preferred horizontal flow.

---

**👤 You:**
> "Identify flow units for a sandstone reservoir with porosity [0.2, 0.21, 0.12] and permeability [100, 110, 20]."

**🤖 AI Agent:**
> Two distinct flow units were identified: Unit 1 (high porosity/permeability) and Unit 2 (low porosity/permeability).


## ❓ FAQ

**Q: What kind of data does this model require?**
The model requires petrophysical measurements such as porosity, permeability, and saturation data, along with lithology information for segmentation.

**Q: How can I identify flow units in my reservoir?**
You can use the `identify_flow_units` tool, providing porosity and permeability arrays along with the specific lithology type.

**Q: Can I assess reservoir heterogeneity?**
Yes, the `evaluate_heterogeneity` tool allows you to quantify spatial variation using property data, correlation length, and anisotropy ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-characterization-model](https://vinkius.com/en/ai-agent-connect/reservoir-characterization-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Characterization Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-characterization-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Characterization Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-characterization-model": {
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
