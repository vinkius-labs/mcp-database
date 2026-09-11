# Storage Tank Evaporation Loss Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/storage-tank-evaporation-loss-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Quantify VOC evaporation losses from storage tanks using physical and environmental data.

## Description
This MCP server provides specialized tools to calculate volatile organic compound (VOC) losses from liquid storage tanks. It models the interaction between product volatility and the physical environment to determine standing losses, working losses, and total annual losses. Use `get_product_volatility_profile` to retrieve vapor pressure data, `calculate_standing_losses` for idle tank losses, and `calculate_working_losses` for operational turnover losses.


## Available Tools (4)
- **get_product_volatility_profile**: Get the characteristic vapor behavior of a specific product
- **calculate_standing_losses**: Calculate standing losses for a storage tank
- **calculate_total_annual_loss**: Calculate the total expected annual volume of product lost
- **calculate_working_losses**: Calculate working losses for a storage tank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storage Tank Evaporation Loss Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the vapor pressure profile for Gasoline?"

**🤖 AI Agent:**
> Gasoline has a reference vapor pressure of 45.0 kPa and is classified as High volatility.

---

**👤 You:**
> "Calculate the standing losses for a fixed roof tank with a 10m diameter, 15m height, 45 kPa vapor pressure, 25°C temperature, and 5 m/s wind speed."

**🤖 AI Agent:**
> The calculated standing loss volume is 124.5 cubic meters.

---

**👤 You:**
> "What would be the total annual loss if standing losses are 500 units and working losses are 1200 units, with an environmental factor of 1.2?"

**🤖 AI Agent:**
> The total expected annual loss is 2040.0 units.


## ❓ FAQ

**Q: What is the difference between standing and working losses?**
Standing losses occur when the tank is idle due to thermal breathing and filling displacement. Working losses occur during the operational cycle of filling and emptying the tank.

**Q: How do I find the vapor pressure for my stored product?**
You can use the `get_product_volatility_profile` tool to retrieve the reference vapor pressure and volatility class for common industrial products.

**Q: Does the tool account for weather conditions?**
Yes, the `calculate_standing_losses` tool specifically includes parameters for average temperature and wind speed to ensure accurate modeling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/storage-tank-evaporation-loss-calculator](https://vinkius.com/en/ai-agent-connect/storage-tank-evaporation-loss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storage Tank Evaporation Loss Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `storage-tank-evaporation-loss-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storage Tank Evaporation Loss Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storage-tank-evaporation-loss-calculator": {
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
