# Water Quality Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/water-quality-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Assess water safety for irrigation and livestock using chemical analysis.

## Description
This MCP server provides specialized tools to evaluate water quality for agricultural use. It calculates suitability for irrigation based on FAO guidelines and assesses safety for livestock using established health thresholds. Use `get_irrigation_suitability` to check crop safety, `get_livestock_safety_index` for animal consumption safety, `get_soil_structure_risk` to predict soil degradation, or `get_water_quality_summary` for a complete dual-use report.


## Available Tools (4)
- **get_soil_structure_risk**: Analyzes the risk of soil degradation caused by the sodium-to-calcium/magnesium ratio
- **get_irrigation_suitability**: Determines if water is safe for irrigation based on chemical composition and specific crop sensitivity
- **get_livestock_safety_index**: Evaluates the safety of water for animal consumption using livestock-specific thresholds
- **get_water_quality_summary**: Provides a unified high-level report comparing irrigation and livestock needs for a single water sample


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Quality Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this water safe for sensitive crops? EC: 1.5, SAR: 4, pH: 7.2, Bicarbonate: 50, Chloride: 20, Boron: 0.5"

**🤖 AI Agent:**
> The water is rated as Good for sensitive crops. The overall risk score is low, though monitoring chloride levels is recommended.

---

**👤 You:**
> "Check the livestock safety for water with EC: 2.0, pH: 8.5, Chloride: 150, Nitrate: 10, Boron: 1.0"

**🤖 AI Agent:**
> The water is rated as Caution for livestock due to high chloride levels which may affect palatability.

---

**👤 You:**
> "What is the soil structure risk for SAR: 15, EC: 1.2, Bicarbonate: 100?"

**🤖 AI Agent:**
> The sodicity risk is High. This may lead to reduced soil permeability. It is recommended to apply gypsum to mitigate sodium accumulation.


## ❓ FAQ

**Q: What parameters are required for irrigation assessment?**
To use `get_irrigation_suitability`, you need to provide Electrical Conductivity (EC), Sodium Adsorption Ratio (SAR), pH, bicarbonate, chloride, boron, and the crop sensitivity category.

**Q: Can I check if water is safe for both animals and crops?**
Yes, use the `get_water_quality_summary` tool to receive a unified report that compares irrigation suitability and livestock safety simultaneously.

**Q: How does the tool handle soil degradation risks?**
The `get_soil_structure_risk` tool analyzes the relationship between SAR, EC, and bicarbonate to predict permeability impact and suggest mitigation strategies like applying gypsum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/water-quality-index-calculator](https://vinkius.com/ai-agent-connect/water-quality-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Quality Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-quality-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Quality Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-quality-index-calculator": {
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
