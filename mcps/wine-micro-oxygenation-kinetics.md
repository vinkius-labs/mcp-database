# Wine Micro-oxygenation Kinetics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-micro-oxygenation-kinetics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Models oxygen consumption and phenolic evolution during micro-oxygenation.

## Description
This MCP server provides advanced kinetic modeling for the micro-oxygenation (MOX) process in winemaking. It allows AI agents to predict how dissolved oxygen levels change over time using `get_dissolved_oxygen_profile`, estimate the extent of phenolic binding with `predict_phenolic_polymerization`, and evaluate sensory impacts via `assess_sensory_evolution`. Additionally, the `optimize_mox_parameters` tool helps determine the ideal oxygen dose rate and duration to achieve specific target styles like Supple, Structured, or Fruit-Forward.


## Available Tools (4)
- **assess_sensory_evolution**: 
- **get_dissolved_oxygen_profile**: 
- **optimize_mox_parameters**: 
- **predict_phenolic_polymerization**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Micro-oxygenation Kinetics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the dissolved oxygen profile look like if I use a dose rate of 0.5 mg/L/h for 24 hours at 15°C with an initial DO of 0.2 mg/L?"

**🤖 AI Agent:**
> The dissolved oxygen concentration will start at 0.2 mg/L and follow a profile where the level increases due to the 0.5 mg/L/h dose rate, while simultaneously being consumed by the phenolic reaction at 15°C, eventually reaching a steady state determined by the kinetics.

---

**👤 You:**
> "How much phenolic polymerization will occur for a 2-year-old wine with 200 mg/L phenolic content at a dose rate of 0.3 mg/L/h and 18°C?"

**🤖 AI Agent:**
> The predicted polymerization index is 0.65 with a color stability score of 0.78 based on the provided phenolic content and temperature.

---

**👤 You:**
> "Find the best MOX settings for a structured wine with 250 mg/L initial phenolics at 16°C."

**🤖 AI Agent:**
> To achieve a Structured style, the optimal dose rate is 0.45 mg/L/h with a duration of 36 hours, providing a predicted stability score of 0.82.


## ❓ FAQ

**Q: How can I use this to stabilize wine color?**
You can use `predict_phenolic_polymerization` to estimate how oxygen exposure will drive the binding of anthocyanins and tannins, which is key to color stability.

**Q: Can I optimize the process for a specific wine style?**
Yes, the `optimize_mox_parameters` tool is designed to find the best dose rate and duration for styles such as Supple, Structured, or Fruit-Forward.

**Q: Does temperature affect the predictions?**
Yes, temperature is a critical input for `get_dissolved_oxygen_profile` and `predict_phenolic_polymerization` as it directly influences the reaction kinetics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-micro-oxygenation-kinetics](https://vinkius.com/en/ai-agent-connect/wine-micro-oxygenation-kinetics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Micro-oxygenation Kinetics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-micro-oxygenation-kinetics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Micro-oxygenation Kinetics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-micro-oxygenation-kinetics": {
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
