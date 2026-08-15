# Mass Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mass-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect market reversals and momentum bulges using the Donald Dorsey Mass Index.

## Description
This MCP server provides deterministic technical analysis tools for identifying market reversals. By calculating the Mass Index, it detects periods of volatility compression followed by explosive price movements. Use `calculate_mass_index` to generate the indicator series, `detect_reversal_signals` to find specific trigger and confirmation zones, and `identify_bulge_formations` to spot sustained momentum builds.


## Available Tools (3)
- **calculate_mass_index**: Calculates the deterministic Mass Index series based on provided price data and smoothing parameters
- **detect_reversal_signals**: Identifies specific price reversal setups based on the Mass Index movement through threshold zones
- **identify_bulge_formations**: Detects periods of sustained high Mass Index values, indicating intense momentum builds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mass Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Mass Index for these high prices [150, 152, 151, 153, 155] and low prices [148, 149, 147, 150, 152]."

**🤖 AI Agent:**
> The Mass Index series has been calculated based on the provided price ranges.

---

**👤 You:**
> "Are there any reversal signals in this Mass Index series: [25.0, 28.0, 27.5, 26.0]?"

**🤖 AI Agent:**
> Yes, a reversal signal was detected at index 3.

---

**👤 You:**
> "Find any bulge formations in this series: [28.0, 29.0, 28.5, 24.0]."

**🤖 AI Agent:**
> A bulge formation was identified from index 0 to index 2 with a duration of 3.


## ❓ FAQ

**Q: What is the Mass Index?**
The Mass Index is a momentum oscillator that identifies market reversals by measuring volatility compression using smoothed price ranges.

**Q: How do I detect a reversal?**
You can use the `detect_reversal_signals` tool to identify when the Mass Index crosses above the upper threshold and subsequently falls below the lower threshold.

**Q: What is a bulge formation?**
A bulge is a period of sustained high Mass Index values, which can be identified using the `identify_bulge_formations` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mass-index-calculator](https://vinkius.com/mcp/mass-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mass Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mass-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mass Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mass-index-calculator": {
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
