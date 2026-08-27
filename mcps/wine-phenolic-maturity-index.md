# Wine Phenolic Maturity Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-phenolic-maturity-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate phenolic maturity, extractability, and harvest timing for grapes.

## Description
This MCP server provides enologists with precise analytical tools to synchronize sugar ripeness with phenolic development. By analyzing berry weight, seed browning, anthocyanins, and tannins, the server calculates critical maturity indices. Use `calculate_maturity_indices` to determine the harvest window status and style potential, `evaluate_harvest_urgency` to estimate days remaining until peak ripeness, and `predict_wine_profile` to forecast the sensory characteristics like color intensity and tannin structure. It also provides variety-specific benchmarks via `get_maturity_thresholds` to ensure optimal harvest decisions.


## Available Tools (4)
- **predict_wine_profile**: Predicts the sensory characteristics of the resulting wine based on the phenolic/sugar balance
- **calculate_maturity_indices**: Performs the core calculation of maturity scores and extractability metrics from raw grape data
- **evaluate_harvest_urgency**: Determines how much time the grower has before the grape profile degrades or reaches peak ripeness
- **get_maturity_thresholds**: Retrieves the standard benchmark values for specific grape varieties to compare against current analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Phenolic Maturity Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the maturity indices for grapes with 22 Brix, 45% seed browning, 1.2 mg/g anthocyanin, and 0.5 seed tannin, with a berry weight of 1.5g."

**🤖 AI Agent:**
> The phenolic maturity score is 0.75, the extractability index is 0.65, the current harvest window is Optimal, and the predicted style is Structured/Bold.

---

**👤 You:**
> "What is the predicted wine profile for grapes with 1.5 mg/g anthocyanin, 0.8 seed tannin, and 24 Brix?"

**🤖 AI Agent:**
> The predicted profile is Deep color intensity, Firm tannin structure, Full body weight, and a Rich/Fruit-forward flavor profile.

---

**👤 You:**
> "How many days until optimal harvest if current Brix is 21 and target Brix is 24, with a maturity score of 0.5?"

**🤖 AI Agent:**
> There are approximately 7 days remaining until the ideal balance is met, with a Moderate risk level.


## ❓ FAQ

**Q: How do I determine if my grapes are ready for harvest?**
You can use the `calculate_maturity_indices` tool to compare current phenolic maturity scores against Brix levels to identify the optimal harvest window.

**Q: Can I predict the wine's body and color?**
Yes, the `predict_wine_profile` tool uses anthocyanin and tannin data to forecast color intensity, tannin structure, and body weight.

**Q: How much time is left before the grapes degrade?**
The `evaluate_harvest_urgency` tool provides an estimate of days remaining until the ideal balance is met and assesses the risk level of delaying harvest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-phenolic-maturity-index](https://vinkius.com/ai-agent-connect/wine-phenolic-maturity-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Phenolic Maturity Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-phenolic-maturity-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Phenolic Maturity Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-phenolic-maturity-index": {
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
