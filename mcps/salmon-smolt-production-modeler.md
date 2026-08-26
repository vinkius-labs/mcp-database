# Salmon Smolt Production Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/salmon-smolt-production-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [predictive-analytics](../categories/predictive-analytics.md)

Predictive modeling for Atlantic salmon smoltification and transfer optimization.

## Description
This MCP server provides a predictive modeling engine for optimizing Atlantic salmon smolt production in freshwater environments. It uses a degree-day accumulation model to forecast developmental milestones, determine optimal seawater transfer windows, and evaluate feeding efficiency. Users can simulate the impact of photoperiod manipulation on smoltification timing and predict survival probabilities based on physiological readiness and thermal history. Key tools include `predict_smoltification_milestones` for forecasting growth and `calculate_optimal_transfer_window` for maximizing seawater survival.


## Available Tools (4)
- **predict_smoltification_milestones**: Predicts when a batch of salmon will reach specific developmental milestones
- **simulate_photoperiod_impact**: Forecasts how altering light cycles will shift the timing of smoltification
- **calculate_optimal_transfer_window**: Determines the best time to move salmon from freshwater to seawater to maximize survival
- **evaluate_feeding_efficiency**: Analyzes how different feeding regimes impact the accumulation of thermal units and growth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salmon Smolt Production Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the smoltification milestones for eggs of 4mm size with a temperature profile of 8 degrees Celsius, 16h photoperiod, and a feeding rate of 1.5%."

**🤖 AI Agent:**
> The predicted date of physiological maturity is October 12th, 2024, with a projected size of 120g and an estimated condition factor of 1.2.

---

**👤 You:**
> "What is the optimal transfer window for salmon needing a 200g target weight and a minimum condition factor of 1.1?"

**🤖 AI Agent:**
> The optimal transfer window is from June 15th to June 30th, with a predicted survival probability of 92%.

---

**👤 You:**
> "How will changing the photoperiod from 12h to 16h affect the smoltification date?"

**🤖 AI Agent:**
> Increasing the photoperiod to 16h will accelerate the process, shifting the new smolt date forward by 14 days.


## ❓ FAQ

**Q: How does the model predict smoltification timing?**
The model uses degree-day accumulation, which calculates growth based on thermal units (temperature multiplied by time) and photoperiod cues.

**Q: Can I use this to find the best time for seawater transfer?**
Yes, you can use `calculate_optimal_transfer_window` to find the specific period where salmon meet both target weight and physiological maturity requirements.

**Q: How is fish health evaluated?**
The model estimates health using the condition factor and a proxy for gill Na+/K+ ATPase activity based on thermal and growth history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/salmon-smolt-production-modeler](https://vinkius.com/ai-agent-connect/salmon-smolt-production-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salmon Smolt Production Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salmon-smolt-production-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salmon Smolt Production Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salmon-smolt-production-modeler": {
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
