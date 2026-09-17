# Wine Optimal Drinking Window MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-optimal-drinking-window)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Predict the ideal consumption period for wine based on chemical composition and storage.

## Description
This MCP server provides analytical tools to model the chemical evolution of wine. By analyzing tannin structure, acidity, alcohol, and phenolic development, it predicts the precise chronological window for consumption. Use `get_drinking_window` to find the peak maturity years, `get_maturity_analysis` to evaluate structural balance and texture, `compare_vintage_profiles` to assess aging potential between years, and `get_storage_impact` to simulate how different environments like cellaring affect the aging curve.


## Available Tools (4)
- **compare_vintage_profiles**: Compares two different vintages of the same wine type to see how they differ in aging potential
- **get_drinking_window**: Determines the specific timeframes for consumption based on a wine's profile
- **get_maturity_analysis**: Provides a deep dive into the specific chemical components driving the wine's current state
- **get_storage_impact**: g. Cellared vs Room Temp) affects its aging.

Calculates how changing storage conditions will shift the drinking window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Optimal Drinking Window** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is the best time to drink this 2015 Cabernet Sauvignon? It has high tannins, medium acidity, 14.5% alcohol, and is currently cellared."

**🤖 AI Agent:**
> The optimal drinking window for this Cabernet Sauvignon is between 2022 and 2035, with the peak maturity expected around 2028.

---

**👤 You:**
> "What is the maturity analysis for a young white wine with low tannins and high acidity?"

**🤖 AI Agent:**
> The wine shows high structural balance due to the acidity, with a high fruit intensity and a texture score reflecting its youthful, crisp nature.

---

**👤 You:**
> "How will my wine's aging change if I move it from room temperature to a cellar?"

**🤖 AI Agent:**
> Moving the wine to a cellar will extend the total drinking window and delay the peak maturity year, providing a more stable environment for slow evolution.


## ❓ FAQ

**Q: How does this tool determine the drinking window?**
The tool uses an aging curve model that considers the interaction between tannins, acidity, and alcohol to predict when a wine reaches its peak and when it begins to decline.

**Q: Can I simulate the effect of moving my wine to a cellar?**
Yes, you can use `get_storage_impact` to calculate how changing storage conditions, such as moving from room temperature to a cellar, will extend the drinking window.

**Q: Does it work for both red and white wines?**
Yes, the tools support Red, White, and Rosé wine types, applying different baseline aging trajectories for each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-optimal-drinking-window](https://vinkius.com/en/ai-agent-connect/wine-optimal-drinking-window)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Optimal Drinking Window** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-optimal-drinking-window` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Optimal Drinking Window** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-optimal-drinking-window": {
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
