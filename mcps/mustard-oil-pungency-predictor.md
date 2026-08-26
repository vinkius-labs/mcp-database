# Mustard Oil Pungency Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mustard-oil-pungency-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predicts mustard oil pungency, yield, and economic value using myrosinase hydrolysis modeling.

## Description
This MCP server connects AI agents to chemical and economic modeling for mustard oil production. By analyzing seed variety, glucosinolate levels, and moisture, it uses a myrosinase hydrolysis model to predict allyl isothiocyanate (AITC) concentration and the resulting pungency index. It also calculates expected oil yield and evaluates how storage duration impacts precursor stability. Use `get_batch_quality_summary` for a complete report on chemical, physical, and economic metrics of a seed batch.


## Available Tools (4)
- **get_batch_quality_summary**: Provides a comprehensive overview of a batch by combining chemical, physical, and economic metrics
- **get_economic_and_application_profile**: Estimates the commercial value of the oil and suggests the best culinary uses
- **get_pungency_prediction**: Calculates the primary chemical and sensory pungency metrics for a specific mustard seed batch
- **get_yield_and_storage_impact**: Determines the total oil yield and evaluates how storage conditions have affected the precursor stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mustard Oil Pungency Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted pungency for a brown mustard variety with 5% glucosinolate content and 10% moisture using cold press?"

**🤖 AI Agent:**
> The predicted AITC concentration is 12.5 mg/kg with a pungency index of 4500 Scoville units.

---

**👤 You:**
> "Calculate the oil yield and stability loss for yellow mustard with 8% moisture after 4 weeks of storage."

**🤖 AI Agent:**
> The predicted oil yield is 32% and the precursor stability loss due to storage is 4.2%.

---

**👤 You:**
> "Give me a full quality summary for oriental mustard, 7% glucosinolate, 12% moisture, heat assisted, stored for 2 weeks."

**🤖 AI Agent:**
> Summary: Predicted AITC is 18.2 mg/kg, Pungency Score is 5200, Expected Yield is 28%, Commercial Value is $450, and Recommended Use is deep frying.


## ❓ FAQ

**Q: How accurate are the pungency predictions?**
Predictions are based on a myrosinase hydrolysis model that accounts for variety-specific enzyme activity and moisture levels.

**Q: Can I predict the economic value of my oil batch?**
Yes, you can use `get_economic_and_application_profile` to estimate the spice value based on the predicted pungency index and oil yield.

**Q: Does storage duration affect the results?**
Yes, the tool `get_yield_and_storage_impact` specifically models how storage duration reduces precursor stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mustard-oil-pungency-predictor](https://vinkius.com/ai-agent-connect/mustard-oil-pungency-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mustard Oil Pungency Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mustard-oil-pungency-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mustard Oil Pungency Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mustard-oil-pungency-predictor": {
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
