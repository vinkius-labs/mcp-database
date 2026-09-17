# Wine Reductive Aging Prediction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-reductive-aging-prediction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Predict reductive sulfur compound development in bottled wine.

## Description
This MCP server provides predictive analytics for wine cellar management. It estimates the development of reductive faults by modeling sulfur compound kinetics. Using tools like `get_sulfur_development_forecast` and `calculate_optimal_drinking_window`, users can predict H2S and mercaptan concentrations, identify the peak quality timeframe, and assess risk levels based on oxygen transfer rates (OTR) and storage temperatures.


## Available Tools (4)
- **check_sensory_threshold_status**: Determines if the wine has already exceeded acceptable sensory limits for sulfur compounds
- **get_sulfur_development_forecast**: Predicts the concentration of specific sulfur compounds over a defined time period
- **calculate_optimal_drinking_window**: Identifies the timeframe when the wine is at its peak quality before reductive faults occur
- **evaluate_reductive_risk_profile**: Categorizes a wine's risk level regarding reductive aging to prioritize cellar management


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Reductive Aging Prediction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the sulfur development for a wine with OTR of 0.001, initial compounds of 0.5, at 14 degrees Celsius for 24 months."

**🤖 AI Agent:**
> The predicted H2S concentration is 0.85 ppm and the mercaptan concentration is 0.12 ppm, with threshold exceedance expected in 30 months.

---

**👤 You:**
> "What is the optimal drinking window for a wine with OTR 0.002, initial compounds 0.3, and storage at 12 degrees?"

**🤖 AI Agent:**
> The optimal drinking window is between month 12 and month 48.

---

**👤 You:**
> "Is a wine with 0.5 ppm H2S and 0.2 ppm mercaptan considered faulty?"

**🤖 AI Agent:**
> No, the wine is currently within acceptable sensory limits.


## ❓ FAQ

**Q: How does temperature affect the prediction?**
Higher storage temperatures accelerate the chemical kinetics of sulfur compound formation, increasing the risk of reductive faults.

**Q: Can I check if my wine is already faulty?**
Yes, you can use `check_sensory_threshold_status` to determine if current H2S or mercaptan concentrations have exceeded sensory limits.

**Q: What is the purpose of the risk profile tool?**
The `evaluate_reductive_risk_profile` tool categorizes wines into risk levels to help prioritize cellar management and temperature control.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-reductive-aging-prediction](https://vinkius.com/en/ai-agent-connect/wine-reductive-aging-prediction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Reductive Aging Prediction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-reductive-aging-prediction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Reductive Aging Prediction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-reductive-aging-prediction": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
