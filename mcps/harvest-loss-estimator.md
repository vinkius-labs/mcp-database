# Harvest Loss Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/harvest-loss-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Quantify grain harvest losses and get machine adjustment recommendations.

## Description
This MCP server provides precision agriculture tools to quantify grain loss across different harvest stages. Use `calculate_area_loss` to scale field samples to hectares, `calculate_total_harvest_loss` to aggregate pre-harvest, header, and separator losses, and `estimate_economic_impact` to determine financial losses. It also includes `recommend_machine_adjustments` to provide actionable mechanical advice based on the detected loss stage.


## Available Tools (4)
- **calculate_area_loss**: Converts localized sample measurements into standardized loss metrics per hectare
- **calculate_total_harvest_loss**: Aggregates different stages of loss to find the total impact on a specific field
- **estimate_economic_impact**: Determines the financial value lost due to harvesting inefficiencies
- **recommend_machine_adjustments**: Provides actionable mechanical advice based on the type of loss detected


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvest Loss Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I collected 0.5kg of grain from a 2m2 sample. What is the loss per hectare for wheat?"

**🤖 AI Agent:**
> The loss is 125 kg/ha.

---

**👤 You:**
> "My total expected yield was 5000kg, but I lost 100kg at the header and 50kg at the separator. What is my total loss percentage?"

**🤖 AI Agent:**
> Your total loss is 3.0%.

---

**👤 You:**
> "I lost 200kg of corn and the price is $0.20 per kg. How much did I lose financially?"

**🤖 AI Agent:**
> The total financial loss is $40.00.


## ❓ FAQ

**Q: How do I calculate loss from a small sample area?**
You can use the `calculate_area_loss` tool by providing the sample area in square meters and the mass of grain collected.

**Q: Can I find out how much money I am losing?**
Yes, use the `estimate_economic_impact` tool with the total mass of lost grain and the current market price.

**Q: What if my machine is losing too much grain at the header?**
The `recommend_machine_adjustments` tool provides specific mechanical advice based on whether the loss is occurring at the header or the separator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/harvest-loss-estimator](https://vinkius.com/ai-agent-connect/harvest-loss-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvest Loss Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harvest-loss-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvest Loss Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvest-loss-estimator": {
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
