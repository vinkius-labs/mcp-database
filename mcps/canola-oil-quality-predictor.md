# Canola Oil Quality Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/canola-oil-quality-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Predict canola oil grade, refining losses, and meal quality from seed characteristics.

## Description
This MCP server provides specialized tools for canola seed analysis. It allows AI agents to determine commercial oil grades using `predict_oil_grade`, estimate processing losses with `estimate_refining_impact`, calculate byproduct nutritional value via `calculate_meal_quality`, and assess economic profitability through `evaluate_crush_margin`. It uses Canadian Grain Commission standards to bridge the gap between seed chemical composition and industrial processing outcomes.


## Available Tools (4)
- **estimate_refining_impact**: Predicts the amount of oil lost during processing and the resulting oil quality
- **calculate_meal_quality**: Estimates the nutritional and industrial value of the byproduct (meal)
- **evaluate_crush_margin**: Provides a financial assessment of the processing profitability
- **predict_oil_grade**: Determines the commercial grade of the canola seed based on chemical and physical purity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canola Oil Quality Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the commercial grade for a seed with 0.5% chlorophyll, 0.1% glucosinolates, and 1.5% erucic acid?"

**🤖 AI Agent:**
> The predicted grade is Premium.

---

**👤 You:**
> "Estimate the refining loss for a seed with 0.8% FFA, 1.2% chlorophyll, and 40% oil content."

**🤖 AI Agent:**
> The estimated refining loss is 2.4%.

---

**👤 You:**
> "Calculate the meal quality for a seed with 40% oil content and a crude protein base of 35%."

**🤖 AI Agent:**
> The estimated crude protein is 38.5% and fiber content is 12.2%.


## ❓ FAQ

**Q: How is the oil grade determined?**
The `predict_oil_grade` tool determines the grade by analyzing chlorophyll levels, glucosinolate concentration, and erucic acid percentage.

**Q: Can I calculate the profitability of a crush?**
Yes, use the `evaluate_crush_margin` tool to calculate the economic margin based on oil grade, refining losses, and current market prices.

**Q: What factors influence refining loss?**
Refining loss is primarily driven by Free Fatty Acid (FFA) levels and chlorophyll content, which can be analyzed using `estimate_refining_impact`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/canola-oil-quality-predictor](https://vinkius.com/ai-agent-connect/canola-oil-quality-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Canola Oil Quality Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `canola-oil-quality-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Canola Oil Quality Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "canola-oil-quality-predictor": {
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
