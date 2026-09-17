# Wine Oxidative Aging Trajectory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-oxidative-aging-trajectory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Models the oxidative aging trajectory of wine using phenolic evolution kinetics.

## Description
This MCP server provides advanced kinetic modeling for wine aging. It allows AI agents to predict how phenolic composition and oxygen exposure influence a wine's evolution. Use `predict_color_evolution` to model visual changes, `simulate_aroma_transition` to track the shift from reductive to oxidative profiles, `calculate_style_timeline` to identify stylistic transitions, and `optimize_aging_window` to determine the ideal duration for achieving specific styles like Sherry or Madeira.


## Available Tools (4)
- **calculate_style_timeline**: Identifies when a wine will transition between different stylistic categories
- **optimize_aging_window**: Calculates the ideal duration to age a wine to reach a specific oxidative style
- **predict_color_evolution**: Predicts how the visual color of the wine will change over a specific timeframe
- **simulate_aroma_transition**: Models the shift from reductive/primary fruit aromas to oxidative/tertiary aromas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Oxidative Aging Trajectory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the color evolution for a wine with 500 initial phenolics, 100 oxygen exposure, at 15 degrees for 365 days."

**🤖 AI Agent:**
> The predicted color shift is amber with an intensity of 0.75, estimated to reach this state in year 1.

---

**👤 You:**
> "When will this wine transition to a Sherry style if it has 400 initial phenolics and 150 oxygen exposure at 18 degrees?"

**🤖 AI Agent:**
> The wine is predicted to transition to the Sherry style in 450 days with a transition probability of 0.85.

---

**👤 You:**
> "What is the optimal aging window for a Madeira style wine with 600 initial phenolics and 200 oxygen exposure at 20 degrees?"

**🤖 AI Agent:**
> The optimal aging duration is 720 days, with a low risk of overoxidation and a predicted deep amber color at peak.


## ❓ FAQ

**Q: How can I predict the color change of my wine?**
You can use the `predict_color_evolution` tool by providing the initial phenolic concentration, oxygen exposure, temperature, and the duration in days.

**Q: Can this tool help me prepare a Sherry style wine?**
Yes, the `optimize_aging_window` tool is specifically designed to calculate the ideal duration to reach target oxidative styles like Sherry.

**Q: How does temperature affect the results?**
Temperature acts as a kinetic multiplier. Higher temperatures accelerate the chemical reactions driven by oxygen exposure, which can be modeled using `simulate_aroma_transition`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-oxidative-aging-trajectory](https://vinkius.com/en/ai-agent-connect/wine-oxidative-aging-trajectory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Oxidative Aging Trajectory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-oxidative-aging-trajectory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Oxidative Aging Trajectory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-oxidative-aging-trajectory": {
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
