# Wine KHT Solubility Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-kht-solubility-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predicts Potassium Bitartrate (KHT) precipitation risks and stabilization needs in wine.

## Description
This MCP server provides specialized tools for enologists to manage Potassium Bitartrate (KHT) stability. By analyzing ethanol levels, pH, temperature, and ionic strength, the server can determine the maximum solubility limit using `get_solubility_limit`. It predicts crystal formation risks with `check_precipitation_risk`, identifies the exact temperature where precipitation begins via `calculate_saturation_temperature`, and estimates the time required for cold stabilization using `estimate_stabilization_duration`.


## Available Tools (4)
- **calculate_saturation_temperature**: Finds the temperature at which the wine's current KHT concentration will begin to precipitate
- **check_precipitation_risk**: Predicts if KHT will precipitate out of the wine at a specific storage temperature
- **estimate_stabilization_duration**: Estimates the time required to perform cold stabilization to reach a safe state
- **get_solubility_limit**: Determines the maximum amount of KHT that can be dissolved in the wine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine KHT Solubility Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum KHT solubility for a wine with 13% ethanol, pH 3.2, temperature 20°C, and ionic strength 0.05?"

**🤖 AI Agent:**
> The maximum solubility limit for this wine composition is 0.45 g/L, with a stability product threshold of 0.2025.

---

**👤 You:**
> "Will my wine precipitate if I store it at 4°C? It has 12% ethanol, pH 3.4, ionic strength 0.04, potassium at 0.02, and bitartrate at 0.03."

**🤖 AI Agent:**
> Yes, there is a high risk of precipitation at 4°C. The saturation degree is 1.25, meaning the current concentration exceeds the solubility limit.

---

**👤 You:**
> "At what temperature will this wine start to precipitate? Ethanol 14%, pH 3.1, ionic strength 0.06, potassium 0.025, bitartrate 0.035."

**🤖 AI Agent:**
> The wine will reach its saturation temperature at 6.5°C.


## ❓ FAQ

**Q: How does ethanol affect KHT solubility?**
Higher ethanol concentrations increase the solubility of KHT, allowing more potassium bitartrate to remain dissolved in the wine matrix.

**Q: Can I use this to plan cold stabilization?**
Yes, you can use `estimate_stabilization_duration` to calculate the time needed to reach a safe target temperature and the expected mass of precipitate.

**Q: What parameters are required for risk assessment?**
To check precipitation risk, you need the ethanol percentage, pH, ionic strength, storage temperature, and the concentrations of potassium and bitartrate ions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-kht-solubility-predictor](https://vinkius.com/ai-agent-connect/wine-kht-solubility-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine KHT Solubility Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-kht-solubility-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine KHT Solubility Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-kht-solubility-predictor": {
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
