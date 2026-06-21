# Yield Curve Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yield-curve-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze interest rate curves, identify spreads, and detect recession signals.

## Description
The Yield Curve Analyzer is a specialized tool for financial professionals to interpret the shape of the yield curve. By using `calculate_curve_metrics`, you can determine if the market is in a Normal, Inverted, Flat, or Humped state and calculate critical spreads like 2s10s and 3m10a. The engine also provides deep insights into economic stability via `examine_recession_risk` to detect potential recessionary signals from yield inversions. Finally, use `get_allocation_guidance` to receive actionable investment strategies and target duration ranges based on the current market environment.


## Available Tools
- **get_allocation_guidance**: Get investment allocation guidance
- **calculate_curve_metrics**: Calculate yield curve metrics
- **examine_recession_risk**: Examine yield curve inversion for recession risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yield Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current state of the yield curve if 3m is 4%, 2y is 4.5%, and 10y is 4.2%?"

**🤖 AI Agent:**
> The yield curve is currently classified as Inverted, with a significant spread inversion detected.

---

**👤 You:**
> "Calculate the spreads for these rates: 3m=3.5%, 6m=3.6%, 1y=3.8%, 2y=4.0%, 5y=4.2%, 10y=4.5%, 30y=4.7%."

**🤖 AI Agent:**
> The classification is Normal, with a 2s10s spread of 0.5000% and a 3m10a spread of 1.0000%.

---

**👤 You:**
> "What strategy should I use if the curve is inverted?"

**🤖 AI Agent:**
> For an Inverted curve, you should follow a Short Duration Strategy with a target duration range focused on lower maturity windows.


## ❓ FAQ

**Q: How can I identify a potential recession using this tool?**
You can use the `examine_recession_risk` tool. It analyzes the spread between 2Y, 10Y, and 3M yields to identify if an inversion depth is high enough to trigger a recession signal.

**Q: What does the `calculate_curve_metrics` tool provide?**
It provides the current classification of the yield curve (e.g., Normal or Inverted) and calculates key market spreads such as 2s10s and 3m10a.

**Q: Can this tool help with bond portfolio management?**
Yes, by using `get_allocation_guidance`, you can receive specific recommendations on whether to shorten or extend your duration based on the identified curve shape.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yield-curve-analyzer](https://vinkius.com/mcp/yield-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yield Curve Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `yield-curve-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yield Curve Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yield-curve-analyzer": {
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
