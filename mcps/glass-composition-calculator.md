# Glass Composition Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/glass-composition-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict glass properties and calculate batch formulations.

## Description
This MCP server provides specialized tools for glass manufacturing and material science. It allows AI agents to calculate precise batch formulations from target oxide compositions using `get_batch_formulation`. Users can predict physical behaviors such as flow resistance with `calculate_viscosity`, estimate thermal expansion via `predict_thermal_properties`, and evaluate the stability of chemical mixes with `analyze_composition_stability` to prevent unwanted crystallization.


## Available Tools (4)
- **calculate_viscosity**: Predicts the flow resistance of a specific glass composition at a specific temperature
- **analyze_composition_stability**: Evaluates if a specific oxide mix will form a stable glass or a crystalline material
- **get_batch_formulation**: Converts a target oxide percentage composition into a practical raw material recipe
- **predict_thermal_properties**: Estimates the thermal expansion behavior of the glass


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glass Composition Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the batch formulation for a composition of 70% SiO2 and 30% Na2O using standard sand and soda ash."

**🤖 AI Agent:**
> To achieve 70% SiO2 and 30% Na2O, you will need 145.2kg of Sand and 62.8kg of Soda Ash for a total batch weight of 208.0kg.

---

**👤 You:**
> "What is the viscosity of a glass with 75% SiO2 at 1200 degrees Celsius?"

**🤖 AI Agent:**
> The predicted viscosity at 1200°C for this composition is 4.52 Pa·s.

---

**👤 You:**
> "Is a composition of 80% SiO2 and 20% CaO stable?"

**🤖 AI Agent:**
> The stability score is 0.92, indicating a highly stable glass with no significant risk of devitrification.


## ❓ FAQ

**Q: How do I calculate a raw material recipe?**
Use the `get_batch_formulation` tool by providing your target oxide percentages and the available raw materials in your inventory.

**Q: Can I predict how the glass will expand?**
Yes, the `predict_thermal_properties` tool estimates the coefficient of thermal expansion and the glass transition temperature.

**Q: How is viscosity determined?**
The `calculate_viscosity` tool predicts flow resistance based on the oxide composition and the specific target temperature provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/glass-composition-calculator](https://vinkius.com/ai-agent-connect/glass-composition-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glass Composition Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glass-composition-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glass Composition Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glass-composition-calculator": {
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
