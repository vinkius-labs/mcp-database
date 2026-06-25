# Crop Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crop-yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate crop productivity in kg/ha and bags/ha using field metrics.

## Description
The Crop Yield Calculator MCP server provides a specialized engine for agricultural productivity analysis. By inputting field parameters such as area, plant density, and grain weight, users can instantly derive yields in both kilograms per hectare and standardized bags per hectare. The server includes tools like `calculate_yield_metrics` to compute mass, `compare_with_benchmark` to evaluate performance against regional historical averages, and `get_crop_standard_weight` to retrieve commodity-specific bag standards (e.g., 60kg for Soybean). It acts as a bridge between raw field data and actionable agricultural insights.


## Available Tools (3)
- **calculate_yield_metrics**: Calculates crop productivity metrics
- **compare_with_benchmark**: Compares calculated yield with regional averages
- **get_crop_standard_weight**: Retrieves the standard bag weight for a crop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crop Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the yield for 10 hectares of Corn with 50,000 plants/ha, 2 ears per plant, and 0.3g grain weight."

**🤖 AI Agent:**
> The yield is 3,000 kg/ha (60 bags/ha), with a total production of 30,000 kg.

---

**👤 You:**
> "How does my yield of 3500 kg/ha in Iowa for Soybean compare to the average?"

**🤖 AI Agent:**
> Your yield is 16.67% above the regional average for Iowa.

---

**👤 You:**
> "What is the standard bag weight for Wheat?"

**🤖 AI Agent:**
> The standard weight for Wheat is 50 kg.


## ❓ FAQ

**Q: How do I calculate my crop yield?**
Use the `calculate_yield_metrics` tool by providing your area in hectares, plant stand per hectare, units per plant, and grain weight in grams.

**Q: Can I compare my results with regional averages?**
Yes, use the `compare_with_benchmark` tool with your state name and crop type to see how your yield deviates from historical norms.

**Q: What are the standard bag weights used?**
The server uses standard weights: 60kg for Soybean and Corn, 50kg for Wheat, and 40kg for Coffee. You can verify any crop using `get_crop_standard_weight`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crop-yield-calculator](https://vinkius.com/mcp/crop-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crop Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crop-yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crop Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crop-yield-calculator": {
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
