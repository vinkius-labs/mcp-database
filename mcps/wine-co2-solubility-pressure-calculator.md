# Wine CO2 Solubility & Pressure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-co2-solubility-pressure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate CO2 solubility, degassing, and bottling pressure in wine using Henry's law.

## Description
This MCP server provides precise calculations for carbon dioxide behavior in wine. It uses Henry's law with corrections for alcohol and sugar content to model gas solubility accurately. Use `calculate_equilibrium_solubility` to find dissolved CO2 levels, `calculate_sparkling_wine_target` to determine required pressures for effervescence, `analyze_still_wine_degassing` to predict CO2 loss during warming, and `predict_bottling_pressure` to estimate future internal bottle pressure based on storage conditions.


## Available Tools (4)
- **analyze_still_wine_degassing**: Predicts how much CO2 will be lost from a still wine during storage or warming
- **calculate_equilibrium_solubility**: Determines the concentration of dissolved CO2 at a specific state
- **calculate_sparkling_wine_target**: Calculates the necessary pressure to achieve a specific level of effervescence
- **predict_bottling_pressure**: Estimates the internal bottle pressure at a later time based on bottling conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine CO2 Solubility & Pressure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the dissolved CO2 concentration in a wine at 12°C, 2 bar pressure, 13% alcohol, and 2 Brix?"

**🤖 AI Agent:**
> The dissolved CO2 concentration is 1.45 g/L with a headspace pressure of 0.55 bar.

---

**👤 You:**
> "How much CO2 will be lost if a still wine with 1.5 g/L CO2 warms from 10°C to 15°C (12% alcohol, 1 Brix)?"

**🤖 AI Agent:**
> The wine will lose 0.22 g/L of CO2, resulting in a final concentration of 1.28 g/L.

---

**👤 You:**
> "What pressure is needed for a sparkling wine at 6°C with 5 g/L CO2, 12% alcohol, and 5 Brix?"

**🤖 AI Agent:**
> The required total pressure is 4.85 bar, with a headspace pressure of 3.12 bar.


## ❓ FAQ

**Q: How does alcohol affect CO2 solubility?**
Alcohol reduces the solubility of CO2 through the salting-out effect, meaning higher alcohol content requires more pressure to hold the same amount of gas.

**Q: Can I predict pressure changes in a bottle during storage?**
Yes, you can use `predict_bottling_pressure` to estimate how internal pressure will change between bottling temperature and storage temperature.

**Q: Does altitude impact the calculations?**
Yes, the tools allow you to input altitude to adjust for changes in atmospheric pressure, which affects the equilibrium of dissolved gases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-co2-solubility-pressure-calculator](https://vinkius.com/en/ai-agent-connect/wine-co2-solubility-pressure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine CO2 Solubility & Pressure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-co2-solubility-pressure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine CO2 Solubility & Pressure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-co2-solubility-pressure-calculator": {
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
