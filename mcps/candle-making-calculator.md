# Candle Making Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/candle-making-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Deterministic formulation engine for precise wax weights, fragrance loads, and wick performance.

## Description
This MCP server provides a deterministic engine for candle makers to calculate exact ingredient weights and burn characteristics. Use `calculate_formulation` to determine the precise mass of wax and fragrance oil needed for any container volume. Use `analyze_wick_performance` to predict melt pool depth and burn hours based on container diameter. Additionally, `predict_shrinkage` helps assess structural risks for pillar candles and container candles by estimating wax contraction during cooling.


## Available Tools (3)
- **analyze_wick_performance**: Recommends a wick series and predicts burn characteristics based on container dimensions
- **calculate_formulation**: Determines the precise weight of wax and fragrance oil required for a specific container and wax type
- **predict_shrinkage**: Estimates the volume loss or structural impact due to wax contraction during cooling


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Candle Making Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 250ml soy wax container and want a 10% fragrance load. How much wax and oil do I need?"

**🤖 AI Agent:**
> For a 250ml soy wax container with a 10% fragrance load, you need 21.5g of fragrance oil and 215g of soy wax, for a total weight of 236.5g.

---

**👤 You:**
> "What is the burn time for a 300g candle using a CD wick series in a 70mm diameter container?"

**🤖 AI Agent:**
> For a 300g candle with a 70mm diameter using the CD wick series, the estimated burn time is 42 hours.

---

**👤 You:**
> "Will a paraffin pillar candle have high shrinkage risk?"

**🤖 AI Agent:**
> Yes, paraffin wax has a higher shrinkage rate (8-12%), and because it is a pillar candle, the structural risk is rated as high.


## ❓ FAQ

**Q: How do I calculate the amount of wax needed for my jar?**
You can use the `calculate_formulation` tool. Provide the container volume, the unit (ml or oz), the wax type, and your desired fragrance load percentage.

**Q: Can this tool help me choose a wick?**
Yes. By using `analyze_wick_performance` with your container diameter and chosen wick series, the engine predicts the optimal wick size and expected burn time.

**Q: How does shrinkage affect my candle?**
Different waxes contract at different rates. Use `predict_shrinkage` to estimate the percentage of volume loss and the structural risk, especially for freestanding pillar candles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/candle-making-calculator](https://vinkius.com/ai-agent-connect/candle-making-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Candle Making Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `candle-making-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Candle Making Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "candle-making-calculator": {
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
