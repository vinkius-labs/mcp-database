# Concrete Shear Friction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-shear-friction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates shear friction capacity and required reinforcement for concrete interfaces using ACI provisions.

## Description
This MCP server provides specialized engineering tools to evaluate the shear transfer capacity of concrete interfaces. It allows users to determine the maximum shear force an interface can resist based on reinforcement area, concrete compressive strength, and joint conditions. Using `calculate_shear_capacity`, engineers can model both monolithic pours and cold joints while accounting for surface roughness. The server also includes `evaluate_safety_factor` to verify design compliance and `determine_required_reinforcement` to solve for the necessary steel area to meet specific shear demands.


## Available Tools (4)
- **compare_interface_conditions**: Evaluates how much capacity is lost when transitioning from a monolithic pour to a cold joint
- **determine_required_reinforcement**: Calculates the minimum steel area required to resist a specific shear load
- **calculate_shear_capacity**: Determines the maximum shear force the interface can resist
- **evaluate_safety_factor**: Checks if the current design is safe against a specific applied load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Shear Friction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the shear capacity for an interface with 500mm² reinforcement, 30MPa concrete, and a 1.2 roughness factor in a monolithic condition?"

**🤖 AI Agent:**
> The calculated shear capacity is 150.0 kN.

---

**👤 You:**
> "Is a design safe if the applied shear is 80kN and the calculated capacity is 100kN?"

**🤖 AI Agent:**
> Yes, the safety factor is 1.25, which is greater than 1.0.

---

**👤 You:**
> "How much reinforcement is needed for a 200kN shear load on a 1000mm² area with 25MPa concrete (monolithic, roughness 1.0)?"

**🤖 AI Agent:**
> The required reinforcement area is 266.67 mm².


## ❓ FAQ

**Q: How does the tool handle monolithic vs cold joint conditions?**
The `calculate_shear_capacity` tool uses a boolean flag to distinguish between a continuous monolithic pour and a separate cold joint, adjusting the capacity based on the expected aggregate interlock and cohesion.

**Q: Can I calculate the required steel area for a specific load?**
Yes, you can use the `determine_required_reinforcement` tool to find the minimum reinforcement area (mm²) needed to resist a target shear force.

**Q: What is the purpose of the roughness factor?**
The roughness factor is a coefficient used in `calculate_shear_capacity` to represent the surface texture, which influences the aggregate interlock and overall shear resistance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-shear-friction-calculator](https://vinkius.com/ai-agent-connect/concrete-shear-friction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Shear Friction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-shear-friction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Shear Friction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-shear-friction-calculator": {
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
