# Nutrient Runoff Loss Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nutrient-runoff-loss-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Simulates nitrogen and phosphorus loss from agricultural fields due to runoff.

## Description
This MCP server provides specialized tools to model nutrient transport from agricultural fields into water bodies. It distinguishes between dissolved and particulate phases for both Nitrogen and Phosphorus, accounting for soil nutrient levels, application rates, and weather conditions. Users can use `calculate_nutrient_loss` to determine specific mass losses, `predict_edge_of_field_loading` to estimate total field impact, and `compare_management_strategies` to evaluate different fertilizer application scenarios. The model also includes `get_incorporation_risk_factor` to assess how delays in soil incorporation increase nutrient vulnerability to rainfall.


## Available Tools (4)
- **calculate_nutrient_loss**: Calculates the mass of specific nutrient losses based on current field conditions and weather
- **compare_management_strategies**: Compares two different application or timing scenarios to determine which results in lower nutrient loss
- **get_incorporation_risk_factor**: Determines the multiplier applied to nutrient loss based on how long nutrients sit on the soil surface
- **predict_edge_of_field_loading**: Predicts the total nutrient mass reaching the field boundary for a specific scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutrient Runoff Loss Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the nutrient loss for a field with 50 units of soil nitrogen, 20 units of soil phosphorus, an application rate of 30 N and 10 P, a 2-day incorporation delay, 15 mm/hr rainfall, and a 3% slope."

**🤖 AI Agent:**
> The calculated losses are: Dissolved N: 12.4, Particulate N: 5.2, Dissolved P: 3.1, Particulate P: 1.8. Total N loss is 17.6 and total P loss is 4.9.

---

**👤 You:**
> "What is the risk factor for a 5-day delay in soil incorporation?"

**🤖 AI Agent:**
> The risk factor for a 5-day delay is 1.45.

---

**👤 You:**
> "Predict the edge-of-field loading for a scenario with 40 soil N, 15 soil P, 25 N application, 5 P application, 0 delay, 10 mm/hr rainfall, and 2% slope."

**🤖 AI Agent:**
> The predicted edge-of-field loading is 8.5 units of Nitrogen and 2.2 units of Phosphorus.


## ❓ FAQ

**Q: How does incorporation timing affect the results?**
A longer delay between fertilizer application and soil incorporation increases the risk of nutrient loss. You can use `get_incorporation_risk_factor` to calculate this specific multiplier.

**Q: Can I compare two different fertilizer plans?**
Yes, the `compare_management_strategies` tool allows you to input two different scenarios to see which one results in lower nitrogen and phosphorus loss.

**Q: What is the difference between dissolved and particulate loss?**
Dissolved loss refers to nutrients soluble in water, while particulate loss refers to nutrients bound to soil particles that are washed away during erosion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nutrient-runoff-loss-model](https://vinkius.com/ai-agent-connect/nutrient-runoff-loss-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutrient Runoff Loss Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutrient-runoff-loss-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutrient Runoff Loss Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutrient-runoff-loss-model": {
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
