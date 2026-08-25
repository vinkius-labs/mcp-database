# Mint Oil Yield Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mint-oil-yield-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict mint oil yield, optimal harvest dates, and chemical quality.

## Description
This MCP server provides specialized tools for mint cultivation management. It allows AI agents to calculate expected essential oil production using `calculate_expected_yield`, determine the best time to harvest with `predict_optimum_harvest`, and assess the commercial grade of the oil via `estimate_oil_quality`. By modeling the relationship between biomass, plant phenology, and environmental factors, it helps optimize mint oil production.


## Available Tools (3)
- **calculate_expected_yield**: Estimates the total expected essential oil yield for a specific field
- **estimate_oil_quality**: Predicts the chemical profile of the oil to assess commercial grade
- **predict_optimum_harvest**: Determines the best date to harvest based on plant maturity and growth stages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mint Oil Yield Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected oil yield for 5000 kg/ha of biomass with a 2% oil concentration and neutral weather?"

**🤖 AI Agent:**
> The expected yield is 100 kg/ha.

---

**👤 You:**
> "When should I harvest if my mint is in the full_bloom stage and 40cm tall with a density of 500 plants/m2?"

**🤖 AI Agent:**
> The recommended harvest date is 2024-07-15.

---

**👤 You:**
> "What will the oil quality be if I harvest at dawn during the budding stage in humid weather?"

**🤖 AI Agent:**
> The predicted quality is Premium with high menthol content.


## ❓ FAQ

**Q: How accurate are the yield predictions?**
Predictions depend on the accuracy of the input biomass and oil percentage. The `calculate_expected_yield` tool provides a confidence score based on the variance of your inputs.

**Q: Can I predict the oil quality?**
Yes, using `estimate_oil_quality`, you can predict menthol and menthone levels to determine if the oil will meet Premium or Standard grades.

**Q: How does weather affect the results?**
Weather impacts are handled via the `weatherImpactFactor` in yield calculations and the `weatherCondition` parameter in quality estimation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mint-oil-yield-predictor](https://vinkius.com/ai-agent-connect/mint-oil-yield-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mint Oil Yield Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mint-oil-yield-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mint Oil Yield Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mint-oil-yield-predictor": {
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
