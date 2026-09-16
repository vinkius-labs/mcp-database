# Wine Barrel Oxygen Transmission MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-barrel-oxygen-transmission)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate oxygen ingress through barrel wood and predict phenolic evolution.

## Description
This MCP server provides specialized tools for enologists and cellar masters to model oxygen ingress in wine barrels. By analyzing wood species, grain tightness, and toasting levels, you can use `calculate_otr` to determine the Oxygen Transmission Rate. The server also allows for long-term planning using `predict_cumulative_uptake` and `analyze_barrel_lifecycle`, and helps predict chemical changes in the wine via `predict_phenolic_evolution`.


## Available Tools (4)
- **analyze_barrel_lifecycle**: Provides a comprehensive summary of a barrel's oxygen performance over its aging cycle
- **calculate_otr**: Calculates the current Oxygen Transmission Rate (OTR) for a specific barrel configuration
- **predict_cumulative_uptake**: Determines the total amount of oxygen that will have entered the wine after a specified duration
- **predict_phenolic_evolution**: Predicts the change in phenolic concentration based on the oxygen exposure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Barrel Oxygen Transmission** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the oxygen transmission rate for a French oak barrel with medium toast at 15 degrees Celsius?"

**🤖 AI Agent:**
> The calculated Oxygen Transmission Rate (OTR) for this configuration is 0.45 mg/L/month.

---

**👤 You:**
> "How much total oxygen will enter a barrel with an OTR of 0.5 mg/L/month over 12 months with a perfect bung seal?"

**🤖 AI Agent:**
> The total cumulative oxygen uptake after 12 months will be 6.0 mg/L.

---

**👤 You:**
> "Predict the phenolic changes for 5 mg/L of oxygen uptake with 200 mg/L initial tannins and 150 mg/L initial anthocyanins."

**🤖 AI Agent:**
> The predicted change is a decrease of 2.5 mg/L in tannins and a decrease of 4.2 mg/L in anthocyanins.


## ❓ FAQ

**Q: How do I calculate the oxygen ingress for a specific oak type?**
You can use the `calculate_otr` tool by providing the wood species, grain tightness, toast level, and storage temperature.

**Q: Can I predict how tannins will change over time?**
Yes, the `predict_phenolic_evolution` tool estimates the change in tannin and anthocyanin concentrations based on total oxygen uptake.

**Q: Does the tool account for barrel aging?**
Yes, the `analyze_barrel_lifecycle` tool models how oxygen permeability evolves as the barrel ages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-barrel-oxygen-transmission](https://vinkius.com/en/ai-agent-connect/wine-barrel-oxygen-transmission)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Barrel Oxygen Transmission** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-barrel-oxygen-transmission` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Barrel Oxygen Transmission** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-barrel-oxygen-transmission": {
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
