# PET Resin Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-resin-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design PET resin production facilities by calculating mass balance, reactor volumes, and SSP requirements.

## Description
This MCP server provides specialized engineering tools for designing Polyethylene Terephthalate (PET) resin plants. It handles the complex chemical transitions from monomers to high-viscosity polymers. Users can use `calculate_mass_balance` to determine feedstock needs, `design_liquid_phase_reactors` to size the esterification, prepolymerization, and finishing stages, and `evaluate_ssp_requirement` to decide if Solid-State Polymerization is needed for high-grade bottle resin. Finally, `generate_plant_summary` aggregates all data into a complete plant configuration report.


## Available Tools (4)
- **generate_plant_summary**: Inputs must be JSON strings.

Aggregates all design data into a single coherent plant configuration report
- **calculate_mass_balance**: Determines the required feedstock amounts to meet a target production capacity
- **design_liquid_phase_reactors**: Sizes the primary melt-phase reactors (Esterification, Prepolymerization, and Finishing)
- **evaluate_ssp_requirement**: Determines if a Solid-State Polymerization (SSP) unit is necessary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PET Resin Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the mass balance for a 100,000 ton capacity plant using PTA with an EG ratio of 1.2."

**🤖 AI Agent:**
> The required feedstock for a 100,000 metric ton capacity plant using PTA and an EG ratio of 1.2 is 85,000 metric tons of PTA and 102,000 metric tons of EG, resulting in a byproduct mass of 17,000 metric tons.

---

**👤 You:**
> "What is the reactor volume needed for a 50,000 ton PTA-based plant with a target IV of 0.8?"

**🤖 AI Agent:**
> For a 50,000 ton capacity plant using PTA and a target IV of 0.8, the required reactor volumes are 450 m³ for esterification, 320 m³ for prepolymerization, and 580 m³ for finishing.

---

**👤 You:**
> "Do I need an SSP unit for a bottle-grade resin with an IV of 0.85?"

**🤖 AI Agent:**
> Yes, for a bottle-grade product with a target IV of 0.85, a Solid-State Polymerization (SSP) unit is required to reach the necessary viscosity.


## ❓ FAQ

**Q: How do I calculate the required amount of PTA and EG?**
You can use the `calculate_mass_balance` tool by providing the target annual capacity, the feedstock type (PTA or DMT), and the required EG ratio.

**Q: When is Solid-State Polymerization (SSP) required?**
SSP is typically required when the target Intrinsic Viscosity (IV) for bottle-grade resin exceeds what can be achieved in the liquid phase. Use `evaluate_ssp_requirement` to confirm.

**Q: Can I design a plant for both fiber and bottle grade resin?**
Yes. By specifying the `productType` as 'fiber' or 'bottle' in the tools, the design calculations for reactor volumes and SSP requirements will adjust accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-resin-plant-designer](https://vinkius.com/en/ai-agent-connect/pet-resin-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PET Resin Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-resin-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PET Resin Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-resin-plant-designer": {
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
