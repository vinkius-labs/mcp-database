# Wine Protein Stability Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-protein-stability-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Quantify protein instability and calculate precise bentonite dosing for wine stabilization.

## Description
This MCP server provides enologists with a suite of analytical tools to manage protein stability in wine. By using `analyze_instability`, users can quantify the risk of protein precipitation based on lab test results. The server then enables precise stabilization planning through `calculate_bentonite_dose`, assesses sensory impact with `evaluate_fining_risk`, and offers alternative stabilization methods via `suggest_alternatives` when overfining is a concern. Additionally, `predict_haze_formation` helps forecast visual clarity during storage.


## Available Tools (5)
- **analyze_instability**: Calculate the primary instability score of a wine based on lab test results
- **calculate_bentonite_dose**: Determine the exact amount of bentonite needed to stabilize the wine
- **evaluate_fining_risk**: Assess the danger of overfining the wine with the calculated bentonite dose
- **predict_haze_formation**: Predict the likelihood of visual haze appearing during the wine's storage
- **suggest_alternatives**: Provide alternative stabilization options when bentonite is not ideal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Protein Stability Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the instability score for a wine with 0.5 protein concentration, a heat test result of 12, an ethanol test result of 8, and a pH of 3.2."

**🤖 AI Agent:**
> The calculated instability score is 42.5, which indicates a high risk of protein precipitation.

---

**👤 You:**
> "How much bentonite is needed for 500 hL of wine with an instability score of 40?"

**🤖 AI Agent:**
> The required bentonite dose is 25.0 g/hL, totaling 12,500 grams for 500 hL of wine.

---

**👤 You:**
> "Predict the haze formation for a wine with an instability score of 35, stored at 15 degrees Celsius for 12 months."

**🤖 AI Agent:**
> There is a 65% probability of visual haze formation during the 12-month storage period.


## ❓ FAQ

**Q: How do I determine if my wine needs bentonite?**
You should first use `analyze_instability` with your lab results (heat and ethanol tests) to get an instability score. If the score indicates high risk, use `calculate_bentonite_dose` to find the required amount.

**Q: What is the risk of using too much bentonite?**
Excessive bentonite can strip wine of desirable characteristics like mouthfeel and aroma. Use `evaluate_fining_risk` to check if your calculated dose poses a high risk to the wine's structure.

**Q: Can I use alternatives to bentonite?**
Yes. If `evaluate_fining_risk` indicates a high risk of overfining, you can use `suggest_alternatives` to receive recommendations for methods like using mannoproteins or chitosan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-protein-stability-analyzer](https://vinkius.com/ai-agent-connect/wine-protein-stability-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Protein Stability Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-protein-stability-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Protein Stability Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-protein-stability-analyzer": {
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
