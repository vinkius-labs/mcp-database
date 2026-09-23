# Grout Quantity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grout-quantity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise grout volumes and masses for construction joints.

## Description
This MCP server provides specialized tools for construction professionals to determine the exact amount of grout needed for joints. Use `get_joint_volume` to find the gap volume, `get_material_density_info` to retrieve density values, `calculate_grout_mass` to convert volume to weight, and `apply_waste_factor` to account for material loss. It connects AI agents to precise geometric and material calculations.


## Available Tools (4)
- **apply_waste_factor**: Adjusts a calculated quantity to include an allowance for material loss
- **calculate_grout_mass**: Converts the calculated joint volume into a required mass (weight)
- **get_joint_volume**: Calculates the total volume of the gap based on linear dimensions
- **get_material_density_info**: Retrieves the standard density values for different types of grout


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grout Quantity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the volume of a joint that is 10m long, 5mm wide, and 10mm deep?"

**🤖 AI Agent:**
> The total volume of the joint is 0.0005 cubic meters.

---

**👤 You:**
> "I have 0.5 cubic meters of volume. How much mass is that if the grout rate is 2.5?"

**🤖 AI Agent:**
> The total mass required is 1.25 units.

---

**👤 You:**
> "Add a 15% waste factor to 10kg of grout."

**🤖 AI Agent:**
> The total quantity including waste is 11.5kg.


## ❓ FAQ

**Q: How do I calculate the total weight of grout needed?**
You can use `get_joint_volume` to find the volume, then use `calculate_grout_mass` with the appropriate material rate to find the weight.

**Q: Does this tool account for material waste?**
Yes, you can use the `apply_waste_factor` tool to add a percentage allowance for spills or uneven depths to your base quantity.

**Q: Where can I find density values for different grout types?**
The `get_material_density_info` tool provides standard density values for various categories like epoxy or cementitious grout.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grout-quantity-calculator](https://vinkius.com/en/ai-agent-connect/grout-quantity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grout Quantity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grout-quantity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grout Quantity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grout-quantity-calculator": {
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
