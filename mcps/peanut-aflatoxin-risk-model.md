# Peanut Aflatoxin Risk Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/peanut-aflatoxin-risk-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-management](../categories/risk-management.md)

Predict aflatoxin contamination risk and economic impact in peanut crops.

## Description
This MCP server provides specialized tools for managing aflatoxin risks in peanut production. It connects AI agents to predictive models that analyze environmental stressors like soil temperature and drought to estimate toxin concentrations. Users can use `predict_contamination_risk` to assess contamination likelihood, `estimate_economic_impact` to project financial losses, `recommend_mitigation_strategy` for harvest and segregation advice, and `validate_regulatory_compliance` to ensure crops meet USA or Europe standards.


## Available Tools (4)
- **estimate_economic_impact**: Calculates the projected financial loss based on the contamination risk
- **predict_contamination_risk**: Calculates the estimated toxin concentration and the likelihood of regulatory non-compliance
- **recommend_mitigation_strategy**: Provides actionable advice on when to harvest and how to sort the crop
- **validate_regulatory_compliance**: Checks if the predicted levels meet the specific requirements of US or European markets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Peanut Aflatoxin Risk Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted aflatoxin risk if soil temperature is 30C, drought stress is 0.5, insect damage is 0.2, harvest is 2 days late, and curing humidity is 60%?"

**🤖 AI Agent:**
> The predicted aflatoxin concentration is 12 ppb with a low risk level.

---

**👤 You:**
> "Will a predicted concentration of 25 ppb be compliant for the USA market?"

**🤖 AI Agent:**
> No, the concentration exceeds the FDA action level for the USA.

---

**👤 You:**
> "What should I do to mitigate risk if the predicted concentration is 15 ppb and I have standard drying facilities?"

**🤖 AI Agent:**
> You should prioritize immediate harvest and implement a segregation strategy to separate high-risk batches.


## ❓ FAQ

**Q: How does the model calculate contamination risk?**
The model uses `predict_contamination_risk` to evaluate cumulative stressors including soil temperature, drought intensity, insect damage, and curing humidity to estimate toxin levels.

**Q: Can I check if my crop is safe for export?**
Yes, you can use the `validate_regulatory_compliance` tool to check predicted levels against USA or Europe regulatory thresholds.

**Q: Does this tool help with financial planning?**
Yes, the `estimate_economic_impact` tool calculates projected financial losses based on predicted toxin concentrations and market prices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/peanut-aflatoxin-risk-model](https://vinkius.com/ai-agent-connect/peanut-aflatoxin-risk-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Peanut Aflatoxin Risk Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `peanut-aflatoxin-risk-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Peanut Aflatoxin Risk Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "peanut-aflatoxin-risk-model": {
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
