# Wine ABV & Fermentation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-abv-fermentation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate alcohol by volume, residual sugar, and fermentation progress.

## Description
This MCP server provides precise tools for winemakers and brewers to monitor fermentation. Use `calculate_fermentation_metrics` to determine actual ABV and sugar depletion, or `estimate_residual_extract` to find remaining solids. It handles both Brix and Specific Gravity measurements, allowing for accurate density corrections during the fermentation process.


## Available Tools (4)
- **convert_measurement_units**: Translates between Brix and Specific Gravity
- **calculate_fermentation_metrics**: Provides a complete overview of the fermentation profile including ABV and sugar depletion
- **estimate_residual_extract**: Determines the concentration of solids remaining in the wine
- **get_fermentation_status**: Interprets the current state of a fermentation process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine ABV & Fermentation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fermentation metrics for an initial gravity of 1.090 and a final gravity of 1.010 at 20 degrees Celsius."

**🤖 AI Agent:**
> The actual ABV is 10.45% and the residual sugar is 2.1%.

---

**👤 You:**
> "What is the status of my fermentation if I started at 12 Brix and I am now at 11.8 Brix?"

**🤖 AI Agent:**
> The fermentation is currently active with 1.6% progress.

---

**👤 You:**
> "Convert 12 Brix to Specific Gravity."

**🤖 AI Agent:**
> 12 Brix is approximately 1.048 Specific Gravity.


## ❓ FAQ

**Q: How do I calculate ABV?**
You can use the `calculate_fermentation_metrics` tool by providing your initial and final readings, the measurement type, and the temperature.

**Q: Can I use Brix readings?**
Yes, all tools support both Brix and gravity measurements via the `convert_measurement_units` logic.

**Q: What is residual sugar?**
Residual sugar is the concentration of fermentable and non-fermentable solids remaining in the liquid, which can be found using `estimate_residual_extract`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-abv-fermentation-calculator](https://vinkius.com/en/ai-agent-connect/wine-abv-fermentation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine ABV & Fermentation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-abv-fermentation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine ABV & Fermentation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-abv-fermentation-calculator": {
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
