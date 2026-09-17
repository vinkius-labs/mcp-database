# Wine Mouthfeel Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-mouthfeel-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predicts sensory mouthfeel attributes of wine based on chemical composition.

## Description
This MCP server provides tools to model the sensory experience of wine. By analyzing chemical inputs like tannin concentration, ethanol, and pH, it uses `predict_astringency` to determine texture quality, `predict_body` to assess weight, and `predict_balance` to evaluate structural equilibrium. It can also use `calculate_texture_score` to provide a holistic mouthfeel metric.


## Available Tools (4)
- **calculate_texture_score**: Provides a single holistic metric for the wine's mouthfeel quality
- **predict_astringency**: Determines the specific quality of the drying sensation (astringency) in the wine
- **predict_balance**: Evaluates the structural equilibrium between acidity and other components
- **predict_body**: Determines the perceived weight or thickness of the wine on the palate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Mouthfeel Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted body of a wine with 13.5% ethanol and 0.5g/L glycerol?"

**🤖 AI Agent:**
> The wine has a medium body with a viscosity score of 0.65.

---

**👤 You:**
> "Predict the astringency for a wine with 0.4 tannin concentration and 0.2 polysaccharide concentration."

**🤖 AI Agent:**
> The predicted astringency is coarse with an intensity of 0.75.

---

**👤 You:**
> "Is a wine with pH 3.5 and titratable acidity 7.0 balanced?"

**🤖 AI Agent:**
> Yes, the wine is balanced with a score of 0.85.


## ❓ FAQ

**Q: What chemical inputs are required?**
To use `predict_body`, you must provide ethanol and glycerol levels. For `predict_balance`, pH and titratable acidity are required.

**Q: How is the texture score calculated?**
The `calculate_texture_score` tool aggregates the results from astringency, body, and balance predictions to produce a single harmony metric.

**Q: Can I predict the specific type of astringency?**
Yes, the `predict_astringency` tool identifies if the sensation is dry, velvety, or coarse based on tannin and polysaccharide levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-mouthfeel-predictor](https://vinkius.com/en/ai-agent-connect/wine-mouthfeel-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Mouthfeel Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-mouthfeel-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Mouthfeel Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-mouthfeel-predictor": {
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
