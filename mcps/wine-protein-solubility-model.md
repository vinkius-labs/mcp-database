# Wine Protein Solubility Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-protein-solubility-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predicts protein stability, haze risk, and bentonite requirements in wine.

## Description
This MCP server provides specialized tools for enologists to model protein behavior in wine. It calculates the heat stability threshold using `analyze_protein_stability`, assesses the likelihood of cloudiness with `predict_haze_risk`, and determines the necessary fining dosage via `calculate_bentonite_requirement`. The model accounts for specific protein fractions like thaumatin-like and chitinase proteins to ensure accurate stability predictions.


## Available Tools (4)
- **analyze_protein_stability**: Evaluates the overall stability of the protein profile under specific environmental conditions
- **calculate_bentonite_requirement**: Estimates the dosage of bentonite needed for protein removal (fining)
- **get_protein_composition_summary**: Provides a breakdown of the protein types to understand the chemical makeup
- **predict_haze_risk**: Determines the likelihood of visible haze forming in the wine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Protein Solubility Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the protein stability for a wine with 300 mg/L protein, 0.6 thaumatin fraction, 0.4 chitinase fraction, pH 3.2, 13% ethanol, and 15°C?"

**🤖 AI Agent:**
> The heat stability threshold is 22.5°C, and the current state is stable with a solubility index of 0.85.

---

**👤 You:**
> "Calculate the haze risk for a wine at 25°C with a stability threshold of 22°C, 400 mg/L protein, and 14% ethanol."

**🤖 AI Agent:**
> The haze risk is Critical with a score of 0.92 due to the temperature exceeding the stability threshold.

---

**👤 You:**
> "How much bentonite is needed for 250 mg/L protein, pH 3.1, and 12.5% ethanol with a 0.5 thaumatin fraction?"

**🤖 AI Agent:**
> The required bentonite dosage is 0.45 g/L, with an expected fining efficiency of 88%.


## ❓ FAQ

**Q: How does this model account for different protein types?**
The model distinguishes between thaumatin-like and chitinase protein fractions to accurately predict how they will react to temperature and ethanol changes.

**Q: Can I use this to plan my fining process?**
Yes, you can use `calculate_bentonite_requirement` to estimate the exact dosage of bentonite needed based on the wine's protein concentration and pH.

**Q: What factors influence the haze risk score?**
The risk score is determined by the current temperature relative to the heat stability threshold, as well as the concentration of ethanol and tannins.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-protein-solubility-model](https://vinkius.com/en/ai-agent-connect/wine-protein-solubility-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Protein Solubility Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-protein-solubility-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Protein Solubility Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-protein-solubility-model": {
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
