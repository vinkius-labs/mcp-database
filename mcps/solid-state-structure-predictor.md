# Solid-State Structure Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/solid-state-structure-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict crystal structures, coordination numbers, and unit cell parameters for inorganic solids.

## Description
This MCP server provides specialized tools for inorganic crystallography. It allows AI agents to predict the most likely coordination geometry using `predict_coordination_geometry`, identify specific crystal templates with `identify_structure_type`, and estimate physical dimensions via `calculate_unit_cell_dimensions`. Additionally, it can evaluate chemical stability using `analyze_composition_stability` based on ionic radii and radius ratio rules. It acts as a bridge between chemical composition data and structural prediction models.


## Available Tools (4)
- **analyze_composition_stability**: Evaluates if a specific chemical composition is likely to form a stable solid based on the ionic radii provided
- **calculate_unit_cell_dimensions**: Estimates the physical size of the unit cell based on the ions and the identified structure
- **identify_structure_type**: Matches a predicted coordination environment to a known crystal structure template
- **predict_coordination_geometry**: Determines the most likely coordination number and geometric arrangement based on the radius ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solid-State Structure Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the coordination geometry for a cation with radius 0.50 and an anion with radius 1.50?"

**🤖 AI Agent:**
> The radius ratio is 0.33, which results in a Tetrahedral coordination geometry.

---

**👤 You:**
> "Is NaCl likely to be stable with a cation radius of 1.02 and anion radius of 1.83?"

**🤖 AI Agent:**
> Yes, the composition is likely stable with a high stability score based on the calculated radius ratio.

---

**👤 You:**
> "What are the unit cell dimensions for a Rock Salt structure with cation radius 0.5 and anion radius 1.5?"

**🤖 AI Agent:**
> The unit cell has an edge length of 3.0 and a cell volume of 27.0.


## ❓ FAQ

**Q: What inputs are required for prediction?**
You need to provide the cation radius and the anion radius to determine the coordination geometry and structure type.

**Q: Can I predict the unit cell size?**
Yes, by using `calculate_unit_cell_dimensions` after identifying the structure type, you can estimate the edge length and volume.

**Q: How is stability determined?**
Stability is assessed by comparing the radius ratio of the ions against known geometric thresholds for stable inorganic structures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/solid-state-structure-predictor](https://vinkius.com/ai-agent-connect/solid-state-structure-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solid-State Structure Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solid-state-structure-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solid-State Structure Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solid-state-structure-predictor": {
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
