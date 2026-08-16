# Ichimoku Cloud Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ichimoku-cloud-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trend-following engine using Ichimoku Cloud indicators.

## Description
This MCP server provides a deterministic execution engine for Ichimoku Cloud trend-following strategies. It calculates all core components including Tenkan-sen, Kijun-sen, Senkou Spans, and the Chikou Span. Use `analyze_ichimoku_signals` to generate precise BUY, SELL, or HOLD signals based on price position, cloud color, and momentum confluence. You can also use `get_cloud_state` to check sentiment or `calculate_signal_strength` to quantify trend intensity.


## Available Tools (3)
- **analyze_ichimoku_signals**: Calculates all Ichimoku components and determines the specific trade signal for every bar in a provided dataset
- **calculate_signal_strength**: Quantifies the intensity of the current trend based on the gap between price and the cloud
- **get_cloud_state**: Provides a focused summary of the cloud's current sentiment and thickness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ichimoku Cloud Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these prices for Ichimoku signals: high=[150, 152, 153], low=[148, 149, 150], close=[149, 151, 152]."

**🤖 AI Agent:**
> The analysis shows a HOLD signal for the provided data points.

---

**👤 You:**
> "What is the current cloud state for these prices?"

**🤖 AI Agent:**
> The cloud is currently bullish with a thickness of 2.5 units.

---

**👤 You:**
> "How strong is the current trend if the price is 5 units above Span A and the cloud thickness is 2?"

**🤖 AI Agent:**
> The trend strength score is high due to the significant distance from the cloud boundary.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the price closes above the cloud, Tenkan-sen is greater than Kijun-sen, the Chikou Span is above the price from 26 bars ago, and the cloud is bullish (Span A > Span B).

**Q: How is signal strength calculated?**
The `calculate_signal_strength` tool determines intensity by evaluating the distance between the current price and the cloud boundary, combined with the thickness of the cloud.

**Q: Can I customize the Ichimoku periods?**
Yes, tools like `analyze_ichimoku_signals` allow you to specify custom periods for Tenkan-sen, Kijun-sen, and Senkou Span B.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ichimoku-cloud-strategy](https://vinkius.com/ai-agent-connect/ichimoku-cloud-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ichimoku Cloud Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ichimoku-cloud-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ichimoku Cloud Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ichimoku-cloud-strategy": {
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
