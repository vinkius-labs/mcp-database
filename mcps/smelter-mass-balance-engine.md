# Smelter Mass Balance Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/smelter-mass-balance-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate mass distributions, metal recoveries, and off-gas compositions for smelting operations.

## Description
This MCP server provides a specialized calculation engine for metallurgical smelting operations. It allows AI agents to perform precise mass balance calculations by determining how elements distribute between matte and slag phases using `calculate_matte_slag_distribution`. Users can evaluate process efficiency with `calculate_metal_recovery`, predict environmental impact via `calculate_offgas_composition`, and optimize flux additions using `simulate_flux_optimization` to control slag viscosity and metal loss.


## Available Tools (4)
- **calculate_matte_slag_distribution**: Determines the mass and elemental distribution between the matte and slag phases
- **calculate_metal_recovery**: Evaluates the efficiency of the smelting operation for specific target metals
- **calculate_offgas_composition**: Predicts the chemical makeup of the gases released during the smelting process
- **simulate_flux_optimization**: Analyzes how varying flux amounts affects the resulting slag composition and matte recovery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smelter Mass Balance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the matte and slag mass for 1000kg of concentrate with 30% copper and 20% iron, using 200kg of silica flux and a copper distribution coefficient of 0.5."

**🤖 AI Agent:**
> The calculation results in a matte mass of 450kg and a slag mass of 750kg, with the copper distributed according to the provided coefficient.

---

**👤 You:**
> "What is the metal recovery if I have 500kg of concentrate (25% Cu) and the resulting matte is 150kg (40% Cu)?"

**🤖 AI Agent:**
> The copper recovery rate is 40.0%.

---

**👤 You:**
> "Predict the off-gas composition for 500kg of concentrate with 30% sulfur and a 0.8 oxidation rate with 1000kg of air."

**🤖 AI Agent:**
> The off-gas will consist of SO2, N2, and O2, with a total gas mass calculated based on the sulfur oxidation and air input.


## ❓ FAQ

**Q: How do I calculate the metal recovery rate?**
You can use the `calculate_metal_recovery` tool by providing the initial concentrate mass and composition, along with the final matte mass and composition.

**Q: Can I predict the gas emissions from the furnace?**
Yes, the `calculate_offgas_composition` tool predicts the chemical makeup of gases like SO2 and N2 based on the sulfur oxidation rate and air input.

**Q: How can I optimize the slag composition?**
Use the `simulate_flux_optimization` tool to analyze how different flux masses affect slag viscosity and metal recovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/smelter-mass-balance-engine](https://vinkius.com/en/ai-agent-connect/smelter-mass-balance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smelter Mass Balance Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smelter-mass-balance-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smelter Mass Balance Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smelter-mass-balance-engine": {
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
