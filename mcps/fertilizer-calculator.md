# Fertilizer Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fertilizer-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise NPK requirements and optimized fertilizer blends.

## Description
This MCP server provides professional-grade agricultural nutrient calculations. It bridges the gap between soil analysis and field application by determining exact nutrient requirements. Use `calculate_nutrient_gap` to find the N, P2O5, and K2O needs based on soil status and crop type. You can also use `convert_nutrient_forms` to switch between elemental and oxide representations, or `recommend_fertilizer_blend` to find the most cost-effective fertilizer combinations for your specific nutrient gap.


## Available Tools (4)
- **calculate_nutrient_gap**: Determines the exact amount of N, P2O5, and K2O that needs to be added to the soil to meet crop requirements
- **convert_nutrient_forms**: Translates between elemental nutrients and their oxide representations
- **get_crop_extraction_data**: Retrieves the theoretical nutrient removal values for a specific crop and yield
- **recommend_fertilizer_blend**: Suggests the most cost-effective combination of available fertilizers to satisfy the calculated nutrient gap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fertilizer Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the nutrient gap for Corn with a target yield of 10 tons/ha, given soil N is 20, P2O5 is 15, and K2O is 10?"

**🤖 AI Agent:**
> The required nutrient gap for Corn is 85.0 kg/ha of Nitrogen, 42.5 kg/ha of P2O5, and 30.0 kg/ha of K2O.

---

**👤 You:**
> "Convert 50 units of elemental Phosphorus to its oxide form."

**🤖 AI Agent:**
> 50 units of elemental Phosphorus is equivalent to 115.0 units of P2O5.

---

**👤 You:**
> "Recommend a blend for a gap of N:20, P2O5:10, K2O:15 using fertilizers: [{"name": "NPK_10_10_10", "n": 10, "p": 10, "k": 10, "cost": 5}, {"name": "High_N", "n": 30, "p": 0, "k": 0, "cost": 8}]"

**🤖 AI Agent:**
> The recommended blend is 2 units of NPK_10_10_10 and 0.33 units of High_N for a total cost of 12.67.


## ❓ FAQ

**Q: How do I calculate the nutrient gap for my crop?**
You can use the `calculate_nutrient_gap` tool. Provide the crop type, target yield, and the current soil nutrient levels to get the exact N, P2O5, and K2O requirements.

**Q: Can I get recommendations for specific fertilizer products?**
Yes. Once you have calculated your nutrient gap, use the `recommend_fertilizer_blend` tool along with your available fertilizer catalog to find the cheapest combination.

**Q: What is the difference between elemental and oxide forms?**
Agricultural products often use oxide forms like P2O5 and K2O. You can use `convert_nutrient_forms` to translate between these and elemental N, P, or K.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fertilizer-calculator](https://vinkius.com/ai-agent-connect/fertilizer-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fertilizer Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fertilizer-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fertilizer Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fertilizer-calculator": {
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
