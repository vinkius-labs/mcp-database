# Wine Mannoprotein Extraction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-mannoprotein-extraction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Predict mannoprotein release and optimize wine stability and mouthfeel.

## Description
This MCP server provides specialized tools for winemakers to predict and optimize the release of mannoproteins from yeast lees. By modeling cell wall degradation kinetics, users can utilize `predict_mannoprotein_release` to calculate expected concentrations based on temperature and stirring frequency. The server also includes tools to `evaluate_sensory_impact` for mouthfeel enhancement, `assess_tartrate_stability` to prevent precipitation, and `optimize_extraction_window` to find the ideal timing for sur lie aging.


## Available Tools (4)
- **evaluate_sensory_impact**: Estimates the qualitative improvements in wine texture and mouthfeel
- **predict_mannoprotein_release**: Calculates the predicted concentration of mannoproteins released from the lees based on environmental conditions
- **assess_tartrate_stability**: Predicts the wine's resistance to potassium bitartrate precipitation
- **optimize_extraction_window**: Recommends the ideal timing and duration for lees contact to maximize quality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Mannoprotein Extraction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted mannoprotein concentration for 48 hours of contact at 15 degrees Celsius with strain Y-202 and 200 RPM stirring?"

**🤖 AI Agent:**
> The predicted mannoprotein concentration is 145.5 mg/L with a stability index of 0.82.

---

**👤 You:**
> "How much will the mouthfeel improve if I reach a concentration of 150 mg/L?"

**🤖 AI Agent:**
> At 150 mg/L, the mouthfeel enhancement is 7.5 and the texture score is 7.2.

---

**👤 You:**
> "I want a mouthfeel score of 8 and stability of 0.9 using strain W-1. What are the optimal settings?"

**🤖 AI Agent:**
> The recommended contact time is 72 hours at 16 degrees Celsius with a stirring frequency of 250 RPM (Mid-Aging window).


## ❓ FAQ

**Q: How can I predict the concentration of mannoproteins?**
You can use the `predict_mannoprotein_release` tool by providing the contact time, temperature, yeast strain, and stirring frequency.

**Q: Can this model help with tartrate stability?**
Yes, the `assess_tartrate_stability` tool predicts the wine's resistance to potassium bitartrate precipitation based on mannoprotein levels.

**Q: How do I find the best time for sur lie aging?**
Use the `optimize_extraction_window` tool to receive recommendations for contact time and temperature based on your target mouthfeel and stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-mannoprotein-extraction-model](https://vinkius.com/en/ai-agent-connect/wine-mannoprotein-extraction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Mannoprotein Extraction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-mannoprotein-extraction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Mannoprotein Extraction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-mannoprotein-extraction-model": {
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
