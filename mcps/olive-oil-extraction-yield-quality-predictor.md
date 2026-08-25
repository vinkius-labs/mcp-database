# Olive Oil Extraction Yield & Quality Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/olive-oil-extraction-yield-quality-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict olive oil yield, extraction loss, and chemical quality risks based on fruit characteristics and malaxing conditions.

## Description
This MCP server provides advanced modeling for olive oil production. It allows AI agents to calculate expected oil yield and extraction loss using `predict_yield_and_loss`. It also estimates chemical quality risks, such as Free Fatty Acids and peroxide levels, via `predict_quality_risk`. For producers looking to balance output and quality, `optimize_malaxing_params` suggests the ideal temperature and duration for the malaxing stage based on the specific olive variety and extraction method.


## Available Tools (3)
- **predict_quality_risk**: 
- **predict_yield_and_loss**: 
- **optimize_malaxing_params**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Olive Oil Extraction Yield & Quality Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the expected yield for 1 tonne of Arbequina olives with 45% moisture and 20% dry oil content using a two-phase decanter at 25C for 20 minutes."

**🤖 AI Agent:**
> The expected yield is 185.5 kg of oil per tonne, with an extraction loss of 12.2 kg.

---

**👤 You:**
> "What is the quality risk for Koroneiki olives if I malax at 35C for 45 minutes?"

**🤖 AI Agent:**
> The predicted FFA is 0.45% and the peroxide value risk is MEDIUM.

---

**👤 You:**
> "Suggest optimal malaxing settings for Picual olives to get the best quality possible using a three-phase method."

**🤖 AI Agent:**
> The optimal settings are a temperature of 22.5C and a duration of 15 minutes.


## ❓ FAQ

**Q: How accurate are the yield predictions?**
The predictions are based on mathematical models of fruit variety, moisture, and extraction method. Using `predict_yield_and_loss` provides a calculated estimate of kilograms of oil per tonne of fruit.

**Q: Can I optimize for high quality instead of high yield?**
Yes. By using `optimize_malaxing_params` and setting the target quality to 'MAX_QUALITY', the tool will recommend lower temperatures and shorter durations to minimize acidity and oxidation.

**Q: What quality indicators are monitored?**
The server monitors Free Fatty Acids (FFA) and Peroxide Value risk through the `predict_quality_risk` tool to help prevent oil degradation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/olive-oil-extraction-yield-quality-predictor](https://vinkius.com/ai-agent-connect/olive-oil-extraction-yield-quality-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Olive Oil Extraction Yield & Quality Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `olive-oil-extraction-yield-quality-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Olive Oil Extraction Yield & Quality Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "olive-oil-extraction-yield-quality-predictor": {
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
