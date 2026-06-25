# Harvest Loss Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvest-loss-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Quantify physical and financial grain losses during harvest.

## Description
The Harvest Loss Calculator MCP server provides precision tools for estimating grain yield losses throughout the harvesting process. Use `calculate_harvest_impact` to quantify physical and financial losses in bags/ha and currency, `retrieve_crop_benchmark` to find industry standard maximum allowable loss for specific crops, and `assess_harvest_efficiency` to evaluate harvest performance against benchmarks.


## Available Tools (3)
- **retrieve_crop_benchmark**: Provides the industry standard for acceptable loss for a specific crop type
- **assess_harvest_efficiency**: Evaluates whether current actual losses are within acceptable industry limits
- **calculate_harvest_impact**: Calculates the total physical and financial losses resulting from cumulative harvesting inefficiencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvest Loss Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impact of a harvest where I expect 60 bags/ha in a 100-hectare field, with 2% pre-harvest loss, 3% platform loss, and 2% threshing loss, at $25 per bag."

**🤖 AI Agent:**
> The total loss is 7% (7 bags/ha). Across 100 hectares, you lost 700 bags, resulting in a financial loss of $17,500.

---

**👤 You:**
> "What is the maximum acceptable loss for Soybeans?"

**🤖 AI Agent:**
> The industry standard maximum allowable loss for Soybeans is 2%.

---

**👤 You:**
> "Is a 5% total loss in Corn considered efficient?"

**🤖 AI Agent:**
> No, a 5% loss for Corn is currently rated as 'Critical' because it exceeds the industry benchmark.


## ❓ FAQ

**Q: How can I calculate the total financial loss from my harvest?**
Use the `calculate_harvest_impact` tool. Provide your expected yield per hectare, field area, various loss percentages (pre-harvest, platform, and threshing), and the current market price per bag.

**Q: How do I know if my harvest efficiency is acceptable?**
You can use the `assess_harvest_efficiency` tool by providing your crop type and the actual total loss percentage you calculated. It will compare your results against industry benchmarks.

**Q: Where can I find the standard allowable loss for a specific crop?**
Use the `retrieve_crop_benchmark` tool and specify the crop type (e.g., Wheat, Corn, or Soybeans) to get the maximum allowable loss percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvest-loss-calculator](https://vinkius.com/mcp/harvest-loss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvest Loss Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harvest-loss-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvest Loss Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvest-loss-calculator": {
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
