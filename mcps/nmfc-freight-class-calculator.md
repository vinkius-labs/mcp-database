# NMFC Freight Class Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nmfc-freight-class-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Determine NMFC freight class and shipping cost impact using density-based calculations.

## Description
This MCP server provides specialized tools for logistics professionals to calculate National Motor Freight Classification (NMFC) details. Use `calculate_shipping_density` to find the density in pounds per cubic foot (PCF) based on weight and dimensions. Then, use `get_class_from_density` to map that density to its specific NMFC class (ranging from Class 50 to 500). Finally, apply `evaluate_cost_impact` to estimate how the freight class affects your total shipping costs using a base rate per pound.


## Available Tools (3)
- **get_class_from_density**: Maps a calculated density value to its specific NMFC freight class
- **evaluate_cost_impact**: Calculates the estimated shipping cost impact based on freight class and a base rate
- **calculate_shipping_density**: Determines the density of a shipment in pounds per cubic foot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NMFC Freight Class Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the density of a 50lb box that is 12x12x12 inches?"

**🤖 AI Agent:**
> The density for a 50lb package with dimensions 12x12x12 inches is approximately 2.89 pounds per cubic foot (PCF).

---

**👤 You:**
> "What NMFC class corresponds to a density of 30 PCF?"

**🤖 AI Agent:**
> A density of 30 PCF falls into Class 50.

---

**👤 You:**
> "If my base rate is $2.00 per lb, what is the cost impact for Class 250?"

**🤖 AI Agent:**
> For a weight of 100 lbs at a base rate of $2.00 per lb, the estimated total cost for Class 250 is $240.00 (applying a multiplier of 1.2).


## ❓ FAQ

**Q: How do I calculate the density of my shipment?**
You can use the `calculate_shipping_density` tool. Simply provide the weight in pounds and the dimensions (length, width, and height) in inches.

**Q: What is NMFC freight class?**
The National Motor Freight Classification (NMFC) system categorizes commodities based on density, ease of handling, and stability to determine shipping rates.

**Q: How does freight class affect my costs?**
Higher freight classes (lower density) typically involve higher cost multipliers due to the increased space consumption in a trailer. You can use `evaluate_cost_impact` to see this effect.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nmfc-freight-class-calculator](https://vinkius.com/mcp/nmfc-freight-class-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NMFC Freight Class Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nmfc-freight-class-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NMFC Freight Class Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nmfc-freight-class-calculator": {
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
