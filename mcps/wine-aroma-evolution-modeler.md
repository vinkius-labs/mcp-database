# Wine Aroma Evolution Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-aroma-evolution-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predicts chemical transformations of aroma compounds during fermentation and aging.

## Description
This MCP server models the dynamic chemical evolution of wine aromas. It allows AI agents to simulate how grape precursors transform into volatile compounds like esters, thiols, and terpenes during fermentation using `simulate_fermentation_aroma`. Users can forecast long-term scent changes with `predict_aging_evolution`, translate chemical data into sensory profiles via `evaluate_aroma_character`, or find the perfect fermentation settings using `optimize_fermentation_parameters`.


## Available Tools (4)
- **evaluate_aroma_character**: Translates numerical compound concentrations into a qualitative description of the wine's scent profile
- **optimize_fermentation_parameters**: Identifies the ideal temperature and yeast strain to achieve a specific desired aroma profile
- **predict_aging_evolution**: Forecasts how the aroma profile changes over a specific duration of aging
- **simulate_fermentation_aroma**: Predicts the concentrations of volatile compounds immediately following the completion of fermentation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Aroma Evolution Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the aroma profile look like after fermentation if I use an Aromatic yeast strain at 20 degrees Celsius with these precursors: {"aminoAcids": 120, "thiolPrecursors": 90}?"

**🤖 AI Agent:**
> The fermentation will result in high concentrations of esters and thiols, providing a strong tropical and floral scent profile.

---

**👤 You:**
> "How will the wine's scent change after 12 months of aging if it starts with these concentrations: {"esters": 50, "thiols": 30, "terpenes": 20, "higherAlcohols": 10} and oxygen exposure is 0.1?"

**🤖 AI Agent:**
> After 12 months, the ester levels will decrease due to degradation, while the thiol profile will remain relatively stable.

---

**👤 You:**
> "What is the best way to get a fruity aroma profile using these precursors: {"aminoAcids": 100, "thiolPrecursors": 50}?"

**🤖 AI Agent:**
> To maximize fruity notes, it is recommended to use an Aromatic yeast strain at a fermentation temperature of 18 degrees Celsius.


## ❓ FAQ

**Q: How accurate are the fermentation predictions?**
Predictions are based on kinetic models of precursor conversion and yeast metabolic rates for the specified strains.

**Q: Can I optimize for a specific scent profile?**
Yes, you can use `optimize_fermentation_parameters` to identify the best temperature and yeast strain to reach your target aroma.

**Q: Does this model account for aging effects?**
Yes, `predict_aging_evolution` forecasts how concentrations of esters and thiols change over time due to degradation and oxidation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-aroma-evolution-modeler](https://vinkius.com/ai-agent-connect/wine-aroma-evolution-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Aroma Evolution Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-aroma-evolution-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Aroma Evolution Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-aroma-evolution-modeler": {
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
