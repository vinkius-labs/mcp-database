# Grain Moisture & Shrinkage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/grain-moisture-shrinkage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate grain weight loss, water evaporation, and handling shrinkage.

## Description
This MCP server provides precise calculations for grain drying processes. It distinguishes between physical water shrinkage and total shrinkage, which includes handling losses. Use `calculate_water_shrink` to find mass lost to evaporation, or `calculate_total_shrink` to account for both water loss and material loss during handling. You can also use `compare_shrinkage_methods` to quantify the impact of handling on your total yield.


## Available Tools (4)
- **calculate_total_shrink**: Calculate the total mass loss including both water evaporation and handling loss
- **calculate_water_shrink**: Calculate the mass lost solely due to the evaporation of water
- **compare_shrinkage_methods**: Compare the results of the physical water-only shrinkage against the total shrinkage model to quantify handling impact
- **get_grain_type_constants**: Retrieve the specific biological constants required for shrinkage calculations for a given grain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grain Moisture & Shrinkage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the water loss for 1000kg of Corn starting at 25% moisture and drying to 13%."

**🤖 AI Agent:**
> The water removed is 250.0kg, leaving a final mass of 750.0kg, with a shrink percentage of 25.0%.

---

**👤 You:**
> "What is the total shrinkage for 500kg of Wheat from 18% to 12% moisture?"

**🤖 AI Agent:**
> The total mass lost is 54.2kg, resulting in a final mass of 445.8kg and a total shrink percentage of 10.84%.

---

**👤 You:**
> "Compare the shrinkage methods for 2000kg of Soybeans at 15% moisture drying to 11%."

**🤖 AI Agent:**
> The water-only shrink is 10.53%, while the total shrink is 11.25%. The handling impact ratio is 1.07.


## ❓ FAQ

**Q: What is the difference between water shrink and total shrink?**
Water shrink is the mass lost strictly from water evaporation. Total shrink includes both that water loss and the handling loss (material lost during movement).

**Q: Which grain types are supported?**
The server supports standard cereals like Corn, Wheat, and Barley, as well as oilseeds like Soybeans and Sunflower.

**Q: How do I see the impact of handling losses?**
You can use the `compare_shrinkage_methods` tool to see the ratio between physical water loss and total shrinkage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/grain-moisture-shrinkage-calculator](https://vinkius.com/ai-agent-connect/grain-moisture-shrinkage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grain Moisture & Shrinkage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grain-moisture-shrinkage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grain Moisture & Shrinkage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grain-moisture-shrinkage-calculator": {
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
