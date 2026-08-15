# Percentage Volume Oscillator (PVO) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/percentage-volume-oscillator-pvo-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate PVO metrics, signal crossovers, and volume-price divergences.

## Description
This MCP server provides a deterministic toolset for analyzing volume momentum using the Percentage Volume Oscillator (PVO). It allows AI agents to calculate core PVO values, signal lines, and histograms. Users can detect critical technical events such as zero-line crosses, signal crossovers, and price-volume divergences using `identify_pvo_signals`. Additionally, the `compare_with_macd` tool enables comparison between volume momentum and price momentum to validate trends. This is an essential bridge for traders looking to confirm price movements with volume-based indicators.


## Available Tools (3)
- **calculate_pvo_metrics**: Calculate core PVO values, signal line, and histogram
- **compare_with_macd**: Compare volume-based PVO with price-based MACD
- **identify_pvo_signals**: Detect zero-line crosses, signal crossovers, and divergences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percentage Volume Oscillator (PVO) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the PVO metrics for this volume series: [100, 120, 110, 130, 150, 140, 160, 180, 170, 190, 210, 230, 220, 250, 270]"

**🤖 AI Agent:**
> The calculated PVO values, signal line, and histogram for the provided series are: PVO: [0.5, 1.2, 0.8, 1.5, 2.1, 1.8, 2.5, 3.2, 2.8, 3.5, 4.2, 4.8, 4.3, 5.1, 5.8].

---

**👤 You:**
> "Identify any signals in these PVO and Signal values: PVO: [1, 2, 3, 2, 1, 0, -1, -2], Signal: [0, 1, 2, 2, 1, 0, -1, -2], Price: [10, 11, 12, 12, 11, 10, 9, 8]"

**🤖 AI Agent:**
> The analysis detected a bullish signal crossover at index 1 and a bearish zero-line cross at index 5.

---

**👤 You:**
> "Compare the volume momentum with price momentum for these series: PVO: [2, 3, 4, 3, 2], Price: [100, 105, 110, 108, 105]"

**🤖 AI Agent:**
> The correlation score between the PVO and the MACD for the provided series is 0.85, indicating a strong alignment between volume and price momentum.


## ❓ FAQ

**Q: What is the difference between PVO and MACD?**
While MACD uses price data, PVO uses volume data. This allows you to see if price trends are supported by actual volume momentum.

**Q: How do I detect a volume expansion?**
A bullish zero-line cross, where the PVO moves from negative to positive, indicates volume expansion.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/percentage-volume-oscillator-pvo-calculator](https://vinkius.com/mcp/percentage-volume-oscillator-pvo-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Percentage Volume Oscillator (PVO) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `percentage-volume-oscillator-pvo-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Percentage Volume Oscillator (PVO) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "percentage-volume-oscillator-pvo-calculator": {
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
