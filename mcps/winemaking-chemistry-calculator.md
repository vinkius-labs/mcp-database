# Winemaking Chemistry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/winemaking-chemistry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Deterministic chemical calculator for grape juice processing and fermentation management.

## Description
This MCP server provides precise chemical calculations for winemakers to manage fermentation stability and grape juice composition. Use `calculate_must_composition` to analyze current sugar and acidity levels, `calculate_adjustments` to determine exact masses for chaptalization or acid correction, and `calculate_additions` to manage sulfur dioxide (SO2) dosing, yeast nutrients, and hydration requirements.


## Available Tools (3)
- **calculate_additions**: Calculates the requirements for sulfur dioxide (SO2), yeast nutrients, and yeast rehydration
- **calculate_adjustments**: Determines the exact mass of additives needed to reach target chemical levels
- **calculate_must_composition**: Analyzes the current state of the must based on raw laboratory measurements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Winemaking Chemistry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500 liters of must with 20 Brix, pH 3.4, and 6 g/L TA. What is the current composition?"

**🤖 AI Agent:**
> The potential alcohol for your 500 liters of must is 11.0%.

---

**👤 You:**
> "I need to raise the TA of 1000 liters of must from 5 g/L to 7 g/L. How much tartaric acid do I need?"

**🤖 AI Agent:**
> You need to add 20 grams of tartaric acid to reach the target acidity.

---

**👤 You:**
> "Calculate SO2 and yeast needs for 1000 liters of must at pH 3.2, targeting 13% alcohol with Saccharomyces cerevisiae."

**🤖 AI Agent:**
> The required initial SO2 is 50 ppm, pre-fermentation SO2 is 30 ppm, and you will need specific maintenance SO2 to keep molecular SO2 at 0.8 ppm based on your pH.


## ❓ FAQ

**Q: How do I calculate the sugar needed for chaptalization?**
You can use the `calculate_adjustments` tool by providing the current Brix, the target Brix, and the total volume of the must.

**Q: Can this tool help with sulfur dioxide (SO2) management?**
Yes, the `calculate_additions` tool calculates initial, pre-fermentation, and maintenance SO2 doses based on your pH and target alcohol.

**Q: How is the potential alcohol calculated?**
The potential alcohol is derived from the current Brix level using the `calculate_must_composition` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/winemaking-chemistry-calculator](https://vinkius.com/ai-agent-connect/winemaking-chemistry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Winemaking Chemistry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `winemaking-chemistry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Winemaking Chemistry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "winemaking-chemistry-calculator": {
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
